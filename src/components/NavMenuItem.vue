<template>
  <li class="hover:text-white">
    <a :href="href">
      <slot></slot>
    </a>
  </li>
</template>

<script setup>

const props = defineProps(['href'])
</script>

