<template>
  <input :id="props.id" type="text">
</template>

<script setup lang="ts">
  const props = defineProps({
    id: String
  })
</script>