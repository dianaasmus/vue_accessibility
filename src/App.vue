<script setup lang="ts">
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <div class="flex flex-col justify-center p-5">
    <header>
      <a href="https://vuejs.org/" hreflang="en">
        <span class="relative block h-10 max-w-10">
          <img alt="Vue logo" src="./assets/logo.svg" />
        </span>
        <span class="sr-only">Visit the Vue.js homepage</span>
      </a>
    </header>

    <main>
      <TheWelcome />
    </main>
  </div>
</template>
