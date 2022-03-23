<template>
<header>
  <div class="container">
    <img src="../assets/img/dc-logo.png" alt="logo">
    <ul>
      <li v-for="(link, index) in links" :class="activeIndex == index ? 'active_index' : ''" v-bind:key="index" @click="setIndex(index)"><a href="#">{{ link.text }}</a></li>
    </ul>
  </div>
</header>
</template>

<script>
/* eslint-disable */
export default {
  name: 'HeaderComics',
  data () {
    return {
      activeIndex: 1,
      links: [{
        text: 'CHARACTERS'
      },
      {
        text: 'COMICS'
      },
      {
        text: 'MOVIES'
      },
      {
        text: 'TV'
      },
      {
        text: 'GAMES'
      },
      {
        text: 'COLLECTIBLES'
      },
      {
        text: 'VIDEOS'
      },
      {
        text: 'FANS'
      },
      {
        text: 'NEWS'
      },
      {
        text: 'SHOP'
      }]
    }
  },
  methods: {
    setIndex(index) {
      this.activeIndex = index;
    }
  }
}
</script>

<style scoped lang="scss">
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    img {
      width: 60px;
      margin: .75rem 0;
    }

    li {
      display: inline-block;
      line-height: 1rem;
      padding: 2.375rem 0;
      border-bottom: solid 5px transparent;

      &.active_index {
      border-bottom: solid 5px #0282F9;
      }

      a {
        line-height: 1rem;
        padding: 2.375rem .75rem;
        text-decoration: none;
        font-size: 10px;
      }
    }
  }
</style>
