<template>
  <div :class="`rounded-md px-2 py-1 text-xs font-semibold ${colorToClassMap[color]}`">
    {{ tag }}
  </div>
</template>

<script setup>
import { colorToClassMap } from '@/utils/colorToClassMap';

const props = defineProps(['color', 'tag']);
</script>
