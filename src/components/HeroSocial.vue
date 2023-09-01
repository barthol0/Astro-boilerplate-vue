<template>
  <img :src="src" :alt="alt" loading="lazy" class="h-12 w-12 hover:translate-y-1" />
</template>

<script setup>
const props = defineProps(['src', 'alt']);
</script>
