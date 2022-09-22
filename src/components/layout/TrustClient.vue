<script setup lang="ts">
const clientAlts = ["CA CIB", "Nexity", "Bouygues Immobilier", "CA Immobilier"];
</script>

<template>
  <div class="trust-client">
    <p>
      <span class="orange"
        >Grâce à Neomi, plus de 500 professionnels de toutes tailles</span
      >
      <br />
      de la promotion immobilière optimisent leur activité
    </p>
    <ul>
      <li v-for="i in 4" :key="i" class="logo-client">
        <img
          :src="`/static/clients/client${i}\.png`"
          :alt="'Logo ' + clientAlts[i]"
        />
      </li>
    </ul>
  </div>
</template>

<style scoped>
.trust-client {
  margin-top: 32px;
  margin-bottom: 16px;
}

p {
  font-weight: 600;
  line-height: 40px;
  font-size: 18px;
  text-align: center;
  padding: 12px;
}

ul {
  display: flex;
  justify-content: space-evenly;
  max-width: 800px;
  margin: 20px auto;
}

.logo-client img {
  height: 36px;
  width: 100%;
}

@media (min-width: 480px) {
  .trust-client {
    margin-top: 64px;

    margin-bottom: 32px;
  }
  .logo-client img {
    height: 64px;
  }
}
</style>
