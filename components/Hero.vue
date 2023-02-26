<template>
  <div class="Hero container">
    <div class="text-container">
      <h1 class="header">Find your Extinguisher</h1>
      <p class="snippet">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod provident
        harum molestias voluptate hic recusandae. Ducimus ut voluptatum,
        obcaecati necessitatibus, ratione aliquam iure rerum saepe culpa vero
        debitis, laudantium nihil.
      </p>
      <button class="button btn btn-danger">Start Looking</button>
    </div>
    <img src="~assets/svg/fire-extinguisher.svg" alt="" class="image" />
  </div>
</template>

<script>
import { mapState } from "vuex";
export default {
  computed: {
    ...mapState(["data1"]),
  },
};
</script>

<style scoped>
.Hero {
  height: 60vh;
  position: relative;
  display: flex;
  padding: 5rem 0;
  align-items: flex-start;
  justify-content: space-between;
}
.text-container {
  width: 50%;
  margin-top: 4rem;
}
.header {
  font-weight: 900;
  font-size: 5rem;
}
.snippet {
  color: gray;
  font-size: 1.25rem;
}
.overly {
  background: rgb(0, 0, 0);
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
}
</style>
