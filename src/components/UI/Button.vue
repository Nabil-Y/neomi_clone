<!-- eslint-disable vue/multi-word-component-names -->

<script setup lang="ts"></script>

<template>
  <button>
    <slot>Demander une démo</slot>
  </button>
</template>

<style scoped>
button {
  height: 40px;
  max-width: 182px;
  padding: 0 12px;

  color: var(--color-white);
  background: var(--color-primary);

  border: solid 1px var(--color-primary);
  cursor: pointer;

  font-weight: 600;
  font-size: 14px;
  font-family: inherit;
}

button:hover {
  background: var(--color-primary-hover);
}
</style>
