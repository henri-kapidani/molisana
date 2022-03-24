<template>
  <div class="card">
    <img :src="cardSrc" :alt="cardTitle">
    <h2>{{ cardTitle }}</h2>
  </div>
</template>

<script>
export default {
  name: 'CardPasta',
  props: {
    cardSrc: String,
    cardTitle: String
  }
}
</script>

<style scoped lang="scss">
  .card {
    flex-basis: calc(25% - .2rem);
    padding: 1rem;
    background-color: white;
    img {
      width: 100%;
    }
  }
</style>
