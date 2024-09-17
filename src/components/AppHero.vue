<script>
  export default {
    name: 'AppHero',
    data() {
      return {
        icons: [
          { name: 'Digital Comics', img: '../src/assets/img/buy-comics-digital-comics.png' },
          { name: 'DC Merchandise', img: '../src/assets/img/buy-comics-merchandise.png' },
          { name: 'Subscription', img: '../src/assets/img/buy-comics-subscriptions.png' },
          { name: 'Comic Shop Locator', img: '../src/assets/img/buy-comics-shop-locator.png' },
          { name: 'DC Power Visa', img: '../src/assets/img/buy-dc-power-visa.svg' }
        ]
      }
    }
  }
</script>

<template>
  <section id="hero">
    <div class="container-hero d-flex align-items-center container justify-content-between">
      <div v-for="(icon, index) in icons" :key="index">
        <img id="hero-icons" :src="icon.img" :alt="icon.name"> 
        <span class="ms-3">{{ icon.name }}</span>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
#hero {
    background-color: rgb(0,130,249);
    color: white;

    .container-hero {
        height: 180px;

        #hero-icons {
            height: 60px;
        }
    }
}
</style>
