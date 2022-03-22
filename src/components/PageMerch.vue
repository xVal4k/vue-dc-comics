<template>
<div class="merch">
  <div class="container">
    <ul>
      <li v-for="(image, index) in images" v-bind:key="index"><a :href="image.href"><img :src="'../assets/img/' + image.src" :alt="image.alt">{{ image.text }}</a></li>
    </ul>
  </div>
</div>
</template>

<script>
/* eslint-disable */
export default {
  name: 'PageMerch',
  data () {
    return {
      images: [
        {
          href: '#',
          src: 'buy-comics-digital-comics.png',
          text: 'DIGITAL COMICS',
          alt: 'buy-comics'
        },
        {
          href: '#',
          src: 'buy-comics-merchandise.png',
          text: 'DC MERCHANDISE',
          alt: 'dc merchandise'
        },
        {
          href: '#',
          src: 'buy-comics-subscriptions.png',
          text: 'SUBSCRIPTION',
          alt: 'subscription img'
        },
        {
          href: '#',
          src: 'buy-comics-shop-locator.png',
          text: 'COMIC SHOP LOCATOR',
          alt: 'position logo'
        },
        {
          href: '#',
          src: 'buy-dc-power-visa.svg',
          text: 'DC POWER VISA',
          alt: 'visa card'
        },
      ]     
    }
  }
}
</script>

<style scoped lang="scss">
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 7rem;
  img {
    width: 50px;
  }
}

li {
    display: inline-block;
    padding: 2.5rem .5rem;
    a {
      line-height: 1rem;
      text-decoration: none;
      font-size: 10px;
      color: white;
    }
  }
</style>
