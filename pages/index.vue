<template>
  <div>
    <NuxtWelcome />
    <div class="test-value">{{ value }}</div>
  </div>
</template>

<script lang="ts" setup>
import { Ref } from 'vue';

type Value = string;
const value: Ref<Value> = ref('');
</script>

<style lang="scss" scoped>
.test-value {
  cursor: pointer;
  &:hover {
    color: green;
  }
}
</style>