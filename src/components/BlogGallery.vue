<template>
  <div class="grid grid-cols-1 gap-6 md:grid-cols-3">
    <BlogCard v-for="post in postList" :key="post.url" :instance="post" />
  </div>
</template>

<script setup>
import BlogCard from '@/components/BlogCard.vue';

const props = defineProps(['postList']);
</script>
