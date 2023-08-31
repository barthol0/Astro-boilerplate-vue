<template>
  <Section>
    <FooterCopyright :site-name="AppConfig.site_name" />
  </Section>
</template>

<script setup>
import { AppConfig } from '@/utils/AppConfig';
import FooterCopyright from '@/components/FooterCopyright.vue';
import Section from '@/components/Section.vue';
</script>
