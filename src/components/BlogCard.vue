<template>
  <a :href="instance.url" class="hover:translate-y-1">
    <div class="overflow-hidden rounded-md bg-slate-800">
      <div class="aspect-w-3 aspect-h-2">
        <img
          :src="instance.frontmatter.imgSrc"
          :alt="instance.frontmatter.imgAlt"
          loading="lazy"
          class="h-full w-full object-cover object-center"
        />
      </div>
      <div class="px-3 pt-4 pb-6 text-center">
        <h2 class="text-xl font-semibold">{{ instance.frontmatter.title }}</h2>
        <div class="mt-1 text-xs text-gray-400">
          {{ formatDate(instance.frontmatter.pubDate) }}
        </div>
        <div class="mt-2 text-sm">{{ instance.frontmatter.description }}</div>
      </div>
    </div>
  </a>
</template>

<script setup>
import { format } from 'date-fns';

const props = defineProps(['instance']);

const formatDate = (date) => {
  return format(new Date(date), 'LLL d, yyyy');
};
</script>
