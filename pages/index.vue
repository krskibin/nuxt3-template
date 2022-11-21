<template>
  <div class="hello-scss">
    <div class="hello-scss__element text-2xl">
      Hello World, {{ value }}!
    </div>
  </div>
</template>

<script setup lang="ts">
import { Ref } from 'vue';

// Typescript ESLint check;
type Value = string;
const value: Ref<Value> = ref('Hello Nuxt3');
</script>

<style lang="scss" scoped>
.hello-scss {
  &__element {
    @apply hover:text-green-400;
    @apply hover:cursor-pointer;
  }
}
</style>