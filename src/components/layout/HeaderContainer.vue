<script setup lang="ts">
import LogoNeomi from "../svg/LogoNeomi.vue";
import Button from "../UI/Button.vue";
</script>

<template>
  <header>
    <div class="header">
      <div class="header-left">
        <LogoNeomi />
      </div>
      <div class="header-right">
        <nav>
          <span>Déja utilisateur?</span>
          <a href="#">Se connecter</a>
        </nav>
        <Button>Demander une démo</Button>
      </div>
    </div>
  </header>
</template>

<style scoped>
header {
  position: fixed;
  background-color: var(--color-white);
  top: 0;
  left: 0;
  right: 0;
  z-index: 2;
}
.header {
  text-align: center;
  padding: 0 16px;
  font-weight: 600;
  box-shadow: var(--shadow);
}

.header-right {
  display: flex;
  justify-content: center;
  align-items: center;
  padding-bottom: 12px;
}

nav > * {
  margin: 10px;
}

nav span {
  display: none;
}

@media (min-width: 480px) {
  .header {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-content: center;
  }

  .header-right {
    padding: 0;
  }

  nav {
    display: flex;
    justify-content: center;
    align-items: center;
  }
}

@media (min-width: 760px) {
  nav span {
    display: block;
  }

  .header-left {
    padding-left: 64px;
  }
}
</style>
