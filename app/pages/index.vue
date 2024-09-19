<script setup>
definePageMeta({
  requiresAuth: false,
})
</script>

<template>
  <UContainer class="space-y-10 py-10">
    <ULandingCTA
      title="The ultimate Vue quiz to test your knowledge"
      description="Test your Vue.js knowledge with our quiz and get an amazing reward!!!"
      card
      :links="[{ label: 'Get started', color: 'primary', size: 'md' }]"
    />
  </UContainer>
</template>
