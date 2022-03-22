<template>
<div class="footer_links">
  <div class="container">
    <div class="left-side">
      <div class="col">
        <h3>DC COMICS</h3>
        <ul>
          <li v-for="(link, index) in DCCOMICS" v-bind:key="index"><a :href="link.href">{{link.text}}</a></li>
        </ul>
      </div>
      <div class="col">
        <h3>SHOP</h3>
        <ul>
          <li v-for="(link, index) in SHOP" v-bind:key="index"><a :href="link.href">{{link.text}}</a></li>
        </ul>
      </div>
      <div class="col">
        <h3>DC</h3>
        <ul>
          <li v-for="(link, index) in DC" v-bind:key="index"><a :href="link.href">{{link.text}}</a></li>
        </ul>
      </div>
      <div class="col">
        <h3>SITES</h3>
        <ul>
          <li v-for="(link, index) in SITES" v-bind:key="index"><a :href="link.href">{{link.text}}</a></li>
        </ul>
      </div>
    </div>
    <img src="../assets/img/dc-logo.png" alt="logo">
  </div>
</div>
</template>

<script>
/* eslint-disable */
export default {
  name: 'FooterLinks',
  data () {
    return {
      DCCOMICS: [
        {
          href: '#',
          text: 'Characters'
        },
        {
          href: '#',
          text: 'Comics'
        },
        {
          href: '#',
          text: 'Movies'
        },
        {
          href: '#',
          text: 'TV'
        },
        {
          href: '#',
          text: 'Games'
        },
        {
          href: '#',
          text: 'Videos'
        },
        {
          href: '#',
          text: 'News'
        }
      ],
      SHOP: [
        {
          href: '#',
          text: 'Shop DC'
        },
        {
          href: '#',
          text: 'Shop DC Collectibles'
        }
      ],
      DC: [
        {
          href: '#',
          text: 'Tersm Of Use'
        },        
        {
          href: '#',
          text: 'Privacy policy (New)'
        },        
        {
          href: '#',
          text: 'Ad Choices'
        },        
        {
          href: '#',
          text: 'Advertising'
        },        
        {
          href: '#',
          text: 'Jobs'
        },        
        {
          href: '#',
          text: 'Subscriptions'
        },        
        {
          href: '#',
          text: 'Talent Workshops'
        },        
        {
          href: '#',
          text: 'CPSC Certificates'
        },        
        {
          href: '#',
          text: 'Ratings'
        },        
        {
          href: '#',
          text: 'Shop Help'
        },        
        {
          href: '#',
          text: 'Contact Us'
        },        
      ],
      SITES: [
        {
          href: '#',
          text: 'DC'
        },
        {
          href: '#',
          text: 'MAD Magazine'
        },
        {
          href: '#',
          text: 'DC Kids'
        },
        {
          href: '#',
          text: 'DC Universe'
        },
        {
          href: '#',
          text: 'DC Power Visa'
        },
        
      ],

    }
  }
}
</script>

<style scoped lang="scss">
.container {
  display: flex;
  justify-content: space-between;
}

.left-side {
  display: flex;
}

.col {
  margin-right: 2rem;
}

img {
  width: 500px;
  transform: rotate(-30deg);
  opacity: .5;
  position: relative;
  bottom: 100px;
}

li {
  display: block;
  a {
    color: grey;
    text-decoration: none;
    font-size: 12px;
  }
}
</style>
