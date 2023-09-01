<template>
  <Section>
    <HeroAvatar>
      <template #title> Hi there, I'm <GradientText>barthol0</GradientText> 👋 </template>
      <template #description
        >Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus
        <a href="" class="text-cyan-400 hover:underline">malesuada</a> nisi tellus, non imperdiet nisi tempor at. Lorem
        ipsum dolor sit amet, <a href="" class="text-cyan-400 hover:underline">consectetur</a> adipiscing elit, sed do
        eiusmod tempor incididunt ut labore et dolore.</template
      >
      <template #avatar>
        <img class="h-80 w-64" src="/assets/images/avatar.svg" alt="Avatar image" loading="lazy" />
      </template>
      <template v-slot:socialButtons>
        <a href="/">
          <HeroSocial :src="'/assets/images/twitter-icon.png'" :alt="'Twitter icon'" />
        </a>
        <a href="/">
          <HeroSocial :src="'/assets/images/facebook-icon.png'" :alt="'Facebook icon'" />
        </a>
        <a href="/">
          <HeroSocial :src="'/assets/images/linkedin-icon.png'" :alt="'Linkedin icon'" />
        </a>
        <a href="/">
          <HeroSocial :src="'/assets/images/youtube-icon.png'" :alt="'Youtube icon'" />
        </a>
      </template>
    </HeroAvatar>
  </Section>
</template>

<script setup>
import GradientText from '@/components/GradientText.vue';
import HeroAvatar from '@/components/HeroAvatar.vue';
import HeroSocial from '@/components/HeroSocial.vue';
import Section from '@/components/Section.vue';
</script>
