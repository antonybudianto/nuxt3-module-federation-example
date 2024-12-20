<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <button class="app-button" @click="counter++">counter {{ counter }}</button>
</template>

<script setup lang="ts" name="AppButtonFromRemote">
import { ref } from 'vue'

const counter = ref(0)
</script>

<style>
.app-button {
  background: var(--app-button-bg, hsl(200, 75%, 42%));
  padding: 0.5rem 1rem;
  border: none;
  color: white;
  border-radius: 0.25rem;
  cursor: pointer;

  transition-property: background;
  transition-duration: 0.2s;
  transition-timing-function: ease;
}

.app-button:hover {
  background: var(--app-button-bg-hover, hsl(200, 75%, 38%));
}
</style>
