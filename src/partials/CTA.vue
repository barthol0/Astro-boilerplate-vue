<template>
  <Section>
    <Newsletter :description="description">
      <template #title> Subscribe to my <GradientText>Newsletters</GradientText> </template>
    </Newsletter>
  </Section>
</template>

<script setup>
import GradientText from '@/components/GradientText.vue';
import Newsletter from '@/components/Newsletter.vue';
import Section from '@/components/Section.vue';

const description =
  'Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur vero esse non molestias eos excepturi, inventore atque cupiditate.';
</script>
