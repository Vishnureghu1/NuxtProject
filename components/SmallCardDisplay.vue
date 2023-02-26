<template>
  <div class="container">
    <h3 class="header">{{ cardsSection.title }}</h3>
    <div class="card-container">
      {{ card }}
      <SmallCard v-for="card in cardsSection.cards" :key="card" :card="card" />
    </div>
  </div>
</template>

<script>
export default {
  name: "SmallCardDisplay",
  props: ["cardsSection"],
};
</script>

<style></style>
