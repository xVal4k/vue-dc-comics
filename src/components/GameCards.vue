<template>
  <div>
    <img :src="cardSrc" :alt="cardTitle">
    <h4>{{ cardTitle }}</h4>
  </div>
</template>

<script>
export default {
  name: 'GameCards',
  props: {
    cardSrc: String,
    cardTitle: String
  }
}
</script>

<style scoped lang="scss">
div {
  width: calc((100% - 6rem) / 6);
  margin: .5rem;
}
img {
  width: 100%;
  margin-bottom: .5rem;
}
</style>
