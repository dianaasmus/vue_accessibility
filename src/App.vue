<script setup lang="ts">
import TheWelcome from './components/TheWelcome.vue'
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
      </nav>
    </header>

    <main class="p-5 md:p-20">
      <TheWelcome />
    </main>
  </div>
</template>
