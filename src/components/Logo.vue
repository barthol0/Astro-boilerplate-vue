<template>
  <div
    class="flex items-center bg-gradient-to-br from-sky-500 to-cyan-400 bg-clip-text text-xl font-bold text-transparent"
  >
    <slot name="icon" />
    {{ name }}
  </div>
</template>

<script setup>
const props = defineProps(['name']);
</script>
