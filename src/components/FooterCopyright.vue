<template>
  <div class="border-t border-gray-600 pt-5">
    <div class="text-sm text-gray-200">
      © Copyright {{ currentYear }} by {{ siteName }}. Built with ♥ by
      <a
        href="https://creativedesignsguru.com"
        target="_blank"
        rel="noopener noreferrer"
        class="text-cyan-400 hover:underline"
      >
        CreativeDesignsGuru </a
      > and adapted for Vue 3 by 
      <a
        href="https://bartholo.io"
        target="_blank"
        rel="noopener noreferrer"
        class="text-cyan-400 hover:underline"
      >barthol0</a>.
    </div>
  </div>
</template>

<script setup>
const props = defineProps(['siteName'])
const currentYear = new Date().getFullYear();
</script>
