<script>
import TheHeader from "./components/TheHeader.vue";
import TheFooter from "./components/TheFooter.vue";

export default {
  components: {
    TheHeader,
    TheFooter,
  },
  data() {
    return {};
  },
};
</script>


<template>
  <TheHeader />

  <main class="bg-black">
    <div class="container">
      <div class="pt-5 pb-5 text-white">
        --CONTENT GOES HERE--
      </div>
    </div>
  </main>

  <TheFooter></TheFooter>
</template>

<style lang="scss"></style>
