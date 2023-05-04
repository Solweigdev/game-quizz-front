<template>
  <label :for="props.for">
    <slot />
  </label>
</template>

<script setup lang="ts">
  const props = defineProps({
    for: String
  })
</script>

<style scoped>
</style>