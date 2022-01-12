<script setup>
import ThemeSwitcher from './components/theme-switcher/ThemeSwitcher.vue';
</script>

<template>
  <div class="border-b-2 my-25 p-1 border-slate-700 dark:border-slate-400 grid justify-items-end">
    <ThemeSwitcher />
  </div>  
  <div class="pt-5 mx-auto">
    <img alt="Vue logo" src="./assets/logo.png"  class="mx-auto"/>             
    <h5 class="text-slate-700 text-center text-2xl dark:text-slate-400">Hello Vue 3 + Vite + Tailwind</h5>  
  </div>  
</template>
