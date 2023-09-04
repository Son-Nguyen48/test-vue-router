<template>
  <div>Project Detail</div>
  <Teleport to="body">
    <div class="modal">
      <p>Hello from the modal!</p>
      {{ route.params.id }}
      <RouterLink :to="{ name: 'app-project' }">Close</RouterLink>
    </div>
  </Teleport>
</template>

<script setup>
import { useRoute } from 'vue-router'
const route = useRoute()
</script>

<style lang="scss" scoped></style>
