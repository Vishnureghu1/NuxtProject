<template>
  <div>
    <div class="container">
      <Hero />
      <LargeCardDisplay
        v-for="cardInfo in largeCardInfo"
        :key="cardInfo.id"
        :cardSection="cardInfo"
      />
      <SmallCardDisplay
        v-for="cardInfo in smallCardSections"
        :key="cardInfo.id"
        :cardsSection="cardInfo"
      />
    </div>
  </div>
</template>

<script>
import { largeCardSections, smallCardSections } from "@/assets/data.js";
import SmallCardDisplay from "../components/SmallCardDisplay.vue";

export default {
  name: "IndexPage",
  data() {
    return {
      largeCardInfo: largeCardSections,
      smallCardSections: smallCardSections,
    };
  },
  components: { SmallCardDisplay },
};
</script>

<style>
/* .container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.title {
  font-family: Arial, Helvetica, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  word-spacing: 5px;
  padding-bottom: 15px;
}
.links {
  padding-top: 15px;
} */
</style>
