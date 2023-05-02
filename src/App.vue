<template>
  <div>
    <NavBar />
    <RouterView v-slot="{ Component }">
      <component :is="Component" />
    </RouterView>
  </div>
</template>

<script setup lang="ts">
import NavBar from '@/components/NavBar/NavBar.vue'
</script>
