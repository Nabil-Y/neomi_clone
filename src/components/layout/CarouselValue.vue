<script setup lang="ts">
import { Pagination } from "swiper";
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import "swiper/css/pagination";
import ValueBlock from "../UI/ValueBlock.vue";
</script>

<template>
  <swiper
    :modules="[Pagination]"
    :pagination="{ clickable: true }"
    :loop="true"
  >
    <swiper-slide class="value-slide-container">
      <ValueBlock
        title="Pilotage de l’activité via le Tableau de Bord"
        image="/static/graphs/neomi-description-img-1.svg"
        alt="Image tableau de bord"
      >
        <p>La page d'accueil de Neomi permet instantanément:</p>
        <p>
          • D'avoir une
          <span class="orange bold">vision globale de l’activité</span>
        </p>
        <p>
          • D’<span class="orange bold"
            >identifier les actions prioritaires</span
          >
        </p>
        <p>
          • D’optimiser la
          <span class="orange bold"
            >recherche d’une opération ou demande spécifique</span
          >
        </p>
      </ValueBlock>
    </swiper-slide>
    <swiper-slide class="value-slide-container">
      <ValueBlock
        title="Co-construction des actes"
        image="/static/graphs/neomi-description-img-2.svg"
        alt="image co construction des actes"
      >
        <p>
          Neomi met en œuvre une solution
          <span class="orange bold">favorisant la collaboration</span> au sein
          des équipes mais également entre les promoteurs et leurs banques afin
          de
          <span class="orange bold"
            >faciliter et réduire les efforts nécessaires à l’obtention des
            actes</span
          >
          via un mécanisme de dépôt de document et d’échanges de commentaires.
        </p>
      </ValueBlock>
    </swiper-slide>
    <swiper-slide class="value-slide-container">
      <ValueBlock
        title="Notification en temps réel"
        image="/static/graphs/neomi-description-img-3.svg"
        alt="image notification en temps réel"
      >
        <p>
          Tous les événements importants qui ont lieu sur la plateforme génèrent
          des notifications
          <span class="orange bold">mail ou in-app</span>. Les préférences de
          celles-ci sont personnalisables, permettant ainsi de
          <span class="orange bold"
            >s’abonner uniquement aux évènements pertinents</span
          >
          pour obtenir le niveau d’information souhaité dans le cadre de son
          activité.
        </p>
        <p>
          Toutes ces notifications sont
          <span class="orange bold"
            >automatisées et ne nécessitent aucune action humaine.</span
          >
        </p>
      </ValueBlock>
    </swiper-slide>
    <swiper-slide class="value-slide-container">
      <ValueBlock
        title="Partage des états de commercialisation"
        image="/static/graphs/neomi-description-img-4.svg"
        alt="image partage des états de commercialisation"
      >
        <p>
          Le recueil des états de commercialisation est pensé pour traiter de
          <span class="orange bold"
            >grands volumes d’opérations sans effort et au fil de l’eau</span
          >.
        </p>
        <p>
          Seules les informations strictement nécessaires doivent être
          renseignées et un mécanisme d’alertes contribue à la
          <span class="orange bold"
            >qualité et au contrôle de l’information</span
          >
          (livraison Q3-2021).
        </p>
      </ValueBlock>
    </swiper-slide>
    <swiper-slide class="value-slide-container">
      <ValueBlock
        title="Signature électronique"
        image="/static/graphs/neomi-description-img-5.svg"
        alt="image signature électronique"
      >
        <p>
          La signature électronique est
          <span class="orange bold">flexible</span> jusqu’à l’émission de l’acte
          et permet de
          <span class="orange bold">
            s’affranchir des délais et tâches liées aux acheminements
            postaux.</span
          >
        </p>
      </ValueBlock>
    </swiper-slide>
    <swiper-slide class="value-slide-container">
      <ValueBlock
        title="Gestion électronique des documents"
        image="/static/graphs/neomi-description-img-6.svg"
        alt="image gestion électronique des documents"
      >
        <p>
          Le chargement des documents est facilité via un
          <span class="orange bold"
            >module d’Intelligence Artificielle d’aide à la saisie.</span
          >
        </p>
        <p>
          Les documents chargés sur la plateforme sont centralisés au niveau des
          opérations. Ils sont
          <span class="orange bold">stockés de manière sécurisée</span>
          (chiffrement, antivirus,…) et sauvegardés.
        </p>
        <p>
          Leur unicité est contrôlée et
          <span class="orange bold"
            >un système de gestion des versions garantit là aussi la qualité de
            la donnée</span
          >
          ainsi que son partage efficace au sein de vos équipes.
        </p>
      </ValueBlock>
    </swiper-slide>
  </swiper>
</template>

<style scoped>
.swiper {
  margin: 32px 0;
}
.value-slide-container {
  display: flex;
  justify-content: center;
}

.value-slide p {
  margin: 12px 0;
  line-height: 30px;
}
</style>
