<script setup lang="ts">
defineProps<{
  title: string;
  image: string;
  alt: string;
  reversed?: boolean;
}>();
</script>

<template>
  <div class="value-slide">
    <div :class="reversed ? 'text-container reversed' : 'text-container'">
      <div class="title bold">{{ title }}</div>
      <div class="separator"></div>
      <slot></slot>
    </div>
    <div class="img-container">
      <img :src="image" :alt="alt" />
    </div>
  </div>
</template>

<style scoped>
.value-slide {
  cursor: grabbing;
  max-width: 420px;
  padding: 0 16px;
}

.value-slide p {
  margin: 12px;
}

.img-container {
  display: flex;
  justify-content: center;
}

.img-container img {
  max-width: 320px;
  margin-bottom: 24px;
}
.separator {
  background-color: var(--color-primary);
  margin-top: 24px;
  height: 4px;
  width: 64px;
}

.title {
  font-size: 18px;
}

@media (min-width: 1200px) {
  .value-slide {
    display: flex;
    justify-content: space-between;
    max-width: 1200px;
    padding: 80px;
  }
  .reversed {
    order: 2;
  }
  .text-container {
    max-width: 400px;
  }
}
</style>
