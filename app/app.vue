<script setup lang="ts">
import type { HeaderLink, FooterLink } from '#ui-pro/types'

const links: HeaderLink[] = [
  { label: 'Github', to: 'https://github.com/kmilogp8496/quiz' },
  { label: 'About', to: '/about' },
]


const footerLinks: FooterLink[] = [{
  label: 'Nuxt UI',
  to: 'https://ui.nuxt.com'
}, {
  label: 'Nuxt Docs',
  to: 'https://nuxt.com'
}, {
  label: 'Nuxt Hub',
  to: 'https://hub.nuxt.com'
}]

</script>

<template>
  <UHeader :links>
    <template #logo>
      <UIcon name="heroicons-question-mark-circle" />
    </template>

    <template #right>
      <UColorModeButton />

      <UButton
        to="https://github.com/kmilogp8496/quiz"
        target="_blank"
        icon="i-simple-icons-github"
        color="gray"
        variant="ghost"
      />
    </template>
  </UHeader>

  <UMain>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </UMain>

  <UFooter :links="footerLinks" />
</template>
