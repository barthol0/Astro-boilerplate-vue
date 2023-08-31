<template>
  <div class="mx-auto mt-5 max-w-prose">
    <div class="aspect-w-3 aspect-h-2">
      <img
        class="h-full w-full rounded-lg object-cover object-center"
        :src="content.imgSrc"
        :alt="content.imgAlt"
      />
    </div>
    <div class="prose prose-invert mt-8 prose-img:rounded-lg">
      <slot></slot>
    </div>
  </div>
</template>

<script setup>
const props = defineProps(['content','author']);
</script>
