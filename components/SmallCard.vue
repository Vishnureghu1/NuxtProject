<template>
  <Nuxt-link :to="`/products/${card.id}`" class="card-container">
    <img
      :src="require(`@/assets/images/${card.image || 'fe1.jpg'}`)"
      alt="fe"
      class="image"
    />
  </Nuxt-link>
</template>

<script>
export default {
  name: "SmallCard",
  props: ["card"],
};
</script>

<style scoped>
.container {
  padding: 2rem 0;
}
.header {
  font-weight: 700;
  font-size: 1.5rem;
  margin-top: 2rem;
}
.card-container {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
.image {
  width: 100%;
  height: 100%;
}
</style>
