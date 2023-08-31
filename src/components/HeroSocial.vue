<template>
  <img
    :src="src"
    :alt="alt"
    loading="lazy"
    class="h-12 w-12 hover:translate-y-1"
  />
</template>

<script setup>
import { ref } from "vue";

const src = ref("");
const alt = ref("");
</script>
