<template>
  <div class="text-center">
    <h1 class="text-3xl font-bold">{{ title }}</h1>
    <div class="mt-3 text-gray-200">{{ description }}</div>
  </div>
</template>

<script setup>
const props = defineProps(['title', 'description']);
</script>
