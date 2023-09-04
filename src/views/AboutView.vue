<template>
  <div class="about">
    <h1>This is an about page</h1>
    {{ count }}
    <button @click="increment">Increment</button>
  </div>
</template>

<script setup>
import { computed } from 'vue'
import { useMenuStore } from '../stores/menu'
const menuStore = useMenuStore()
const count = computed(() => {
  return menuStore.count
})

const increment = menuStore.increment
</script>
