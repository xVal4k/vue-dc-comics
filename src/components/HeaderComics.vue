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
    }
  }

  .active_index {
    border-bottom: solid 3px #0282F9;
  }  

  li {
    display: inline-block;
    line-height: 5rem;
    a {
      line-height: 1rem;
      padding: 2rem .5rem;
      text-decoration: none;
      font-size: 10px;
    }
  }
</style>
