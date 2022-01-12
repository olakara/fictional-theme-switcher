<script setup>
import IconSun from './IconSun.vue';
import IconMoon from './IconMoon.vue';
import {useColorMode} from '@vueuse/core';

const colorMode = useColorMode();

const switchTheme = () => {
  if (colorMode.value === 'dark') {
    colorMode.value = 'light'
  } else {
    colorMode.value = 'dark'
  } 
}
</script>

<template>
  <button class="m-1">
    <IconSun v-if="colorMode === 'dark'" class="text-yellow-400 text-2xl"  @click="switchTheme"/>
    <IconMoon v-if="colorMode === 'light'" class="text-black-600 text-2xl"  @click="switchTheme"/>
  </button>
</template>

<script>
export default {

}
</script>
