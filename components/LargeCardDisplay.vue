<template>
  <div class="container">
    <h4 class="header">{{ cardSection.title }}</h4>
    <p class="snippet">{{ cardSection.snippet }}</p>
    <div class="cards-container">
      <largeCard
        v-for="card in cardSection.cards"
        :key="card.image"
        :card="card"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "LargeCardDisplay",
  props: ["cardSection"],
};
</script>

<style scoped>
.container {
  margin-top: 2rem;
}
.header {
  font-weight: 700;
  font-size: 1.5rem;
}
.snippet {
  color: gray;
  margin-top: 1.5rem;
}
.cards-container {
  display: flex;
  justify-content: space-between;
}
</style>
