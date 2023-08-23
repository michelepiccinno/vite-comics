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

        <Slide
        v-for="(Card, i) in CardList"
        :key="i"
        :img-src="Card.bgSrc"
        :testo="Card.thumb"
      ></Slide>


      </div>
    </div>
  </main>

</template>

<style lang="scss" scoped>

</style>
