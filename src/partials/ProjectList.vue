<template>
  <Section>
    <template #title>Recent <GradientText>Projects</GradientText></template>
    <div class="flex flex-col gap-6">
      <Project
        v-for="project in projects"
        :key="project.name"
        :name="project.name"
        :description="project.description"
        :link="project.link"
        :img="project.img"
      >
        <template #tags>
          <Tags v-for="(tag, color) in project.category" :key="tag" :color="color" :tag="tag" />
        </template>
      </Project>
    </div>
  </Section>
</template>

<script setup>
import GradientText from '@/components/GradientText.vue';
import Project from '@/components/Project.vue';
import Section from '@/components/Section.vue';
import Tags from '@/components/Tags.vue';

const projects = [
  {
    name: 'Project 1',
    description:
      'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse bibendum. Nunc non posuere consectetur, justo erat semper enim, non hendrerit dui odio id enim.',
    link: '/',
    img: {
      src: '/assets/images/project-web-design.png',
      alt: 'Project Web Design',
    },
    category: {
      FUCHSIA: 'Astro.js',
      LIME: 'Web design',
      SKY: 'Tailwind.css',
      ROSE: 'TypeScript',
    },
  },
  {
    name: 'Project 2',
    description:
      'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse bibendum. Nunc non posuere consectetur, justo erat semper enim, non hendrerit dui odio id enim.',
    link: '/',
    img: {
      src: '/assets/images/project-fire.png',
      alt: 'Project Fire',
    },
    category: {
      VIOLET: 'Next.js',
      EMERALD: 'Blog',
      YELLOW: 'JavaScript',
    },
  },
  {
    name: 'Project 3',
    description:
      'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse bibendum. Nunc non posuere consectetur, justo erat semper enim, non hendrerit dui odio id enim.',
    link: '/',
    img: {
      src: '/assets/images/project-maps.png',
      alt: 'Project Maps',
    },
    category: {
      FUCHSIA: 'Astro.js',
      INDIGO: 'Bootstrap',
      ROSE: 'TypeScript',
    },
  },
];
</script>
