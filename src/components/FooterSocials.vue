<template>
<div class="footer_socials">
  <div class="container">
    <button>SIGN-UP NOW!</button>
    <div class="socials">
      <a href="#">FOLLOW US</a>
      <ul>
        <li v-for="(logo, index) in logos" v-bind:key="index"><a href="#"><img :src="logo.src" :alt="logo.alt"></a></li>
      </ul>
    </div>
  </div>
</div>
</template>

<script>
/* eslint-disable */
import facebook from '../assets/img/footer-facebook.png'
import twitter from '../assets/img/footer-twitter.png'
import youtube from '../assets/img/footer-youtube.png'
import pinterest from '../assets/img/footer-pinterest.png'
import periscope from '../assets/img/footer-periscope.png'

export default {
  name: 'FooterSocials',
  data () {
    return {
      logos: [
        {
          src: facebook,
          alt: 'facebook'
        },
        {
          src: twitter,
          alt: 'twitter'
        },
        {
          src: youtube,
          alt: 'youtube'
        },
        {
          src: pinterest,
          alt: 'pinterest'
        },
        {
          src: periscope,
          alt: 'periscope'
        }
      ]
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
    width: 30px;
    vertical-align: middle;
    margin: 0 .2rem;
  }
}

button {
  padding: .5rem 1rem;
  color: white;
  background: #1C1C1C;
  border: solid 2px #0282F9;
  cursor: pointer;
}

.socials {
  display: flex;
  align-items: center;
}

a {
  text-decoration: none;
  font-size: 20px;
  margin-right: 1.5rem;
  color: #0282F9;
}

li {
  display: inline-block;
  line-height: 4.8rem;
}
</style>
