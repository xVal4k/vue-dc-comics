<template>
<main>
  <div class="container">
    --> Content goes here >--
  </div>
</main>
</template>

<script>
export default {
  name: 'MainCont'
}
</script>

<style scoped lang="scss">
@import '../assets/styles/variables';

.container {
  height: $commongHeight;
  display: flex;
  align-items: center;
  color: white;
}
</style>
