<script setup lang="ts">
import TheWelcome from './components/TheWelcome.vue'
import { ref } from 'vue'

const isOpen = ref(false)

function toggleMenu() {
  isOpen.value = !isOpen.value
}
</script>

<template>
  <div class="flex flex-col justify-center">
    <header class="flex h-20 items-center justify-center">
      <nav>
        <a href="https://vuejs.org/" hreflang="en">
          <span class="relative block h-10 w-10">
            <img alt="Vue logo" src="./assets/logo.svg" />
          </span>
          <span class="sr-only">Visit the Vue.js homepage</span>
        </a>
        <button
          class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-400 transition-all duration-300 ease-in-out hover:text-amber-200"
          @click="toggleMenu"
        >
          <span class="absolute -inset-0.5" />
          <span class="sr-only">Open main menu</span>

          <label class="relative block h-8 w-10 cursor-pointer">
            <input type="checkbox" id="burger" class="peer hidden" />
            <span
              class="absolute left-0 top-0 h-1 w-full origin-left rounded bg-white transition-all duration-300 ease-in-out peer-checked:left-1.5 peer-checked:top-0 peer-checked:rotate-[38deg]"
            ></span>
            <span
              class="absolute left-0 top-1/2 h-1 w-full -translate-y-1/2 rounded bg-white transition-all duration-300 ease-in-out peer-checked:w-0 peer-checked:opacity-0"
            ></span>
            <span
              class="absolute left-0 top-full h-1 w-full origin-left -translate-y-full rounded bg-white transition-all duration-300 ease-in-out peer-checked:left-1.5 peer-checked:top-7 peer-checked:-rotate-[38deg]"
            ></span>
          </label>
        </button>
      </nav>
    </header>

    <main class="p-5 md:p-20">
      <TheWelcome />
    </main>
  </div>
</template>
