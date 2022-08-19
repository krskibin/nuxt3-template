<template>
  <div>
    <NuxtWelcome />
    <div class="test-value">{{ value }}</div>
  </div>
</template>

<script lang="ts" setup>
const value = ref('');
</script>

<style lang="scss" scoped>
.test-value {
  cursor: pointer;
  &:hover {
    color: green;
  }
}
</style>