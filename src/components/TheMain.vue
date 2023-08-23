<script>
export default {
  components: {
    Card,
  },
  props: {
    cardList: {
      type: Array,
      required: true,
    },
  },
  data() {
    return {
      currentCard: 0,
    };
  }
}
</script>

<template>

<main class="bg-black">
      <div class="jumbotron-container">
      </div>
    <div class="container">
      <div class="pt-5 pb-5 text-white">

        --CONTENT GOES HERE--

        <div
        v-for="(Card, i) in cardList"
        :key="i"
        :img-src="Card.bgSrc"
        :testo="Card.thumb"
      ></div>


      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>

</style>
