<template>
<div class="merch">
  <div class="container">
    <ul>
      <li v-for="(image, index) in images" v-bind:key="index"><a :href="image.href"><img :src="image.src" :alt="image.alt">{{ image.text }}</a></li>
    </ul>
  </div>
</div>
</template>

<script>
/* eslint-disable */
import DCOMICS from '../assets/img/buy-comics-digital-comics.png'
import DCMerchandise from '../assets/img/buy-comics-merchandise.png'
import ComicsSubs from '../assets/img/buy-comics-subscriptions.png'
import ShopLocator from '../assets/img/buy-comics-shop-locator.png'
import PowerVisa from '../assets/img/buy-dc-power-visa.svg'

export default {
  name: 'PageMerch',
  data () {
    return {
      images: [
        {
          href: '#',
          src: DCOMICS,
          text: 'DIGITAL COMICS',
          alt: 'buy-comics'
        },
        {
          href: '#',
          src: DCMerchandise,
          text: 'DC MERCHANDISE',
          alt: 'dc merchandise'
        },
        {
          href: '#',
          src: ComicsSubs,
          text: 'SUBSCRIPTION',
          alt: 'subscription img'
        },
        {
          href: '#',
          src: ShopLocator,
          text: 'COMIC SHOP LOCATOR',
          alt: 'position logo'
        },
        {
          href: '#',
          src: PowerVisa,
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
}

img {
  width: 50px;
  vertical-align: middle;
}

li {
  display: inline-block;
  padding: 2.5rem .5rem;
  a {
    line-height: 1rem;
    text-decoration: none;
    font-size: 10px;
    color: white;
    vertical-align: middle;
  }
}
</style>
