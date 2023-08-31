<template>
  <Section>
    <PostHeader :content="content" :author="AppConfig.author" />
    <PostContent :content="content">
      <slot></slot>
    </PostContent>
  </Section>
</template>

<script setup>
import { AppConfig } from '@/utils/AppConfig';
import PostContent from '@/components/PostContent.vue';
import PostHeader from '@/components/PostHeader.vue';
import Section from '@/components/Section.vue';

const props = defineProps(['content']);
</script>
