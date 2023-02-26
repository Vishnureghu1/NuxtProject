<template>
  <div class="container">
    <LargeCardDisplay
      v-for="cardInfo in largeCardInfo.slice(0, 1)"
      :key="cardInfo.id"
      :cardSection="cardInfo"
    />

    <SmallCardDisplay
      v-for="cardInfo in smallCardInfo"
      :key="cardInfo.id"
      :cardSection="cardInfo"
    />
  </div>
</template>

<script>
import LargeCardDisplay from "../../components/LargeCardDisplay.vue";
import { largeCardSections, smallCardSections } from "@/assets/data.js";
import SmallCardDisplay from "../../components/SmallCardDisplay.vue";
export default {
  components: { LargeCardDisplay, SmallCardDisplay },
  data() {
    return {
      largeCardInfo: largeCardSections,
      smallCardInfo: smallCardSections,
    };
  },
};
</script>

<style></style>
