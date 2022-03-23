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

<style>

</style>
