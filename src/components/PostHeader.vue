<template>
  <h1 class="text-center text-3xl font-bold">{{ content.title }}</h1>
  <div class="mt-2 text-center text-sm text-gray-400">By {{ author }} on {{ formattedDate }}</div>
</template>

<script setup>
import { computed } from 'vue';

const props = defineProps(['content', 'author']);

const formattedDate = computed(() => {
  return new Date(props.content.pubDate).toLocaleString('en-US', {
    month: 'long',
    day: 'numeric',
    year: 'numeric',
  });
});
</script>
