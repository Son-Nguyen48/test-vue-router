<template>
  <div>App</div>
  <RouterLink :to="{ name: 'app-project' }">Project</RouterLink>
  <RouterLink :to="{ name: 'app-profile' }">Profile</RouterLink>
  <RouterView />
</template>

<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<style lang="scss" scoped></style>
