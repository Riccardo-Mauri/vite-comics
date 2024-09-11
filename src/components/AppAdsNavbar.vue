<script>
//1- Importazione del componenente necessario che voglio aggiungere qua


export default {
  data() {
    return {
      items: [
        {
          imgSrc: '/public/img/buy-comics-digital-comics.png',
          altText: 'Digital Comics',
          url: '#',
          text: 'DIGITAL COMICS'
        },
        {
          imgSrc: '/public/img/buy-comics-merchandise.png',
          altText: 'DC Merchandise',
          url: '#',
          text: 'DC MERCHANDISE'
        },
        {
          imgSrc: '/public/img/buy-comics-shop-locator.png',
          altText: 'Subscription',
          url: '#',
          text: 'SUBSCRIPTION'
        },
        {
          imgSrc: '/public/img/buy-comics-subscriptions.png',
          altText: 'Comic Shop Locator',
          url: '#',
          text: 'COMIC SHOP LOCATOR'
        },
        {
          imgSrc: '/public/img/buy-dc-power-visa.svg',
          altText: 'DC Power Visa',
          url: '#',
          text: 'DC POWER VISA'
        }
      ]
    }
  },
  //2- Dichiarazione del componente 
  components: {

  },
  methods: {

  }
}
</script>

<template>
  <div class="main-links">
    <div class="container">
      <div class="ads-container">
        <ul>
          <li v-for="(item, index) in items" :key="index">
            <div><img :src="item.imgSrc" :alt="item.altText"></div>
            <div><a :href="item.url">{{ item.text }}</a></div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  max-width: 1300px;
  margin: 0 auto;
  position: relative;
}
.main-links {
  min-height: 150px;
  background-color: #0282F9;
  display: flex;
  align-items: center;
}
.ads-container{
  width: 100%;
}
.ads-container ul {
  display: flex;
  justify-content: space-around;
  list-style: none;
  text-decoration: none;
}

.ads-container ul li {
  width: calc(100% / 5);
  height: 100%;
  display: flex;
  align-items: center;
}

.ads-container ul li img {
  width: 50%;
  height: 50%;
  object-fit: contain;
}
.ads-container ul li a{
  text-decoration: none;
  color: white;
}
</style>
