<template>
  <div>Project</div>
  <RouterLink @click="open = true" :to="{ name: 'app-id-project', params: { id: '123' } }"
    >Go to detail</RouterLink
  >
  <button @click="open = true">Open Modal</button>

  <Teleport to="body">
    <div v-if="open" class="modal">
      <p>Hello from the modal!</p>
      <button @click="open = false">Close</button>
    </div>
  </Teleport>
</template>

<script setup>
import { ref } from 'vue'
import { RouterLink } from 'vue-router'
const open = ref(false)
</script>

<style lang="scss" scoped></style>
