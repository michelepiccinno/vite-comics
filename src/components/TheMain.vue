<script>
export default {
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
      <div class="d-flex row row-cols-6 g-2 pt-5 pb-5 text-white">

        <div class="books-container" v-for="(Card, i) in cardList" :key="i">
          <img class="img-books" :src="Card.thumb" alt="">
          <p class="text-white">{{ Card.series }}</p>
        </div>

      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>
.books-container {
  height: 300px;
  .img-books {
    width: 100%;
  }
}
</style>
