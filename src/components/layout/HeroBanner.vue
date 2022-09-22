<script setup lang="ts">
import Button from "../UI/Button.vue";
</script>

<template>
  <div class="main-hero">
    <div class="slogan">
      <h1>
        Neomi, la plateforme <span class="orange">collaborative</span> pour les
        professionnels de la promotion immobilière
      </h1>
      <Button>Demander une démo</Button>
    </div>
  </div>
</template>

<style scoped>
.main-hero {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  position: relative;
  height: 390px;
  margin-top: 80px;

  text-align: center;

  background-image: url("/static/homepage/hero-banner.jpg");
  background-repeat: repeat-x;
  background-position: 0 40px;
}
.slogan {
  position: absolute;
  z-index: 1;
  max-width: 400px;
  padding: 0 12px;
}

.slogan h1 {
  font-size: 18px;
  line-height: 40px;
  font-weight: 600;
  margin-bottom: 30px;
}

.main-hero::after {
  content: "";
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  background-color: rgba(255, 255, 255, 0.1);
}

@media (min-width: 480px) {
  .main-hero {
    height: 440px;
    margin-top: 80px;
    background-position: 0 -80px;
  }
  .slogan h1 {
    margin-bottom: 50px;
  }
}
</style>
