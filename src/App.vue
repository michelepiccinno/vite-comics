<script>
import TheHeader from "./components/TheHeader.vue";
import TheFooter from "./components/TheFooter.vue";
import TheMain from "./components/TheMain.vue";
import ComiCards from "../src/db/dc-comics.json";

export default {
  components: {
    TheHeader,
    TheFooter,
    TheMain,
  },
  data() {
    return {
      ComiCards
    };
  },
};
</script>


<template>
  <TheHeader />


  <TheMain :card-list="ComiCards">

</TheMain>

  <TheFooter></TheFooter>
</template>

<style lang="scss">
.jumbotron-container {
  height: 400px;
  background-image: url(..//src/assets/img/jumbotron.jpg);
}
</style>
