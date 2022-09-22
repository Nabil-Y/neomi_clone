<script setup lang="ts">
import ValueBlock from "../UI/ValueBlock.vue";
import Button from "../UI/Button.vue";
</script>

<template>
  <div class="value-section">
    <ValueBlock
      title="Axe de valeur promoteur"
      image="/static/homepage/screen1.png"
      alt="image ecran dashboard"
      ><p>
        Allège le montage des dossiers de financements et leur partage à la
        banque.
      </p>
      <p>
        Facilite la mise en place et le suivi des opérations par toutes vos
        équipes.
      </p>
      <Button>Demander une démo</Button>
    </ValueBlock>
    <ValueBlock
      title="Axe de valeur banque"
      image="/static/homepage/screen2.png"
      alt="image ecran dashboard"
      reversed
      ><p>Renforce le suivi des risques via le suivi de commercialisation.</p>
      <p>
        Facilite la gestion des opérations en pool formalisé ou non formalisé.
      </p>
      <Button>Demander une démo</Button></ValueBlock
    >
  </div>
</template>

<style scoped>
.value-section > * {
  margin: 24px auto;
}
.value-section img {
  max-width: 1000px;
}
p {
  margin: 16px 0;
}
button {
  margin: 16px 0;
}
</style>
