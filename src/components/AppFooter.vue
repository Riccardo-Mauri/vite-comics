<script>
//1- Importazione del componenente necessario che voglio aggiungere qua


export default {
  data() {
    return {
         // Dati per DC COMICS
         dcComicsLinks: [
        { title: 'Characters', url: '#' },
        { title: 'Comics', url: '#' },
        { title: 'Movies', url: '#' },
        { title: 'TV', url: '#' },
        { title: 'Games', url: '#' },
        { title: 'Videos', url: '#' },
        { title: 'News', url: '#' }
      ],
      // Dati per il negozio (SHOP)
      shopLinks: [
        { title: 'Shop DC', url: '#' },
        { title: 'Shop DC Collectibles', url: '#' }
      ],
      // Dati per DC
      dcLinks: [
        { title: 'Terms Of Use', url: '#' },
        { title: 'Privacy Policy (New)', url: '#' },
        { title: 'Ad Choices', url: '#' },
        { title: 'Advertising', url: '#' },
        { title: 'Jobs', url: '#' },
        { title: 'Subscriptions', url: '#' },
        { title: 'Talent Workshops', url: '#' },
        { title: 'CPSC Certificates', url: '#' },
        { title: 'Ratings', url: '#' },
        { title: 'Shop Help', url: '#' },
        { title: 'Contact Us', url: '#' }
      ],
      // Dati per Sites
      sitelinks: [
        { title: 'DC', url: '#' },
        { title: 'Mad Magazine', url: '#' },
        { title: 'Dc Kids', url: '#' },
        { title: 'Dc Universe', url: '#' },
        { title: 'DC Power visa', url: '#' },
      ],
      socialLinks: [
        {
          url: '#',
          imgSrc: '/img/footer-facebook.png',
          altText: 'Facebook'
        },
        {
          url: '#',
          imgSrc: '/img/footer-periscope.png',
          altText: 'Periscope'
        },
        {
          url: '#',
          imgSrc: '/img/footer-pinterest.png',
          altText: 'Pinterest'
        },
        {
          url: '#',
          imgSrc: '/img/footer-youtube.png',
          altText: 'YouTube'
        },
        {
          url: '#',
          imgSrc: '/img/footer-twitter.png',
          altText: 'Twitter'
        }
      ],

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
  <footer>
    <div class="top-footer">
      <div class="container">
        <div class="link-footer-top">
          <div>
            <h4>
              DC COMICS
            </h4>
            <ul>
              <li v-for="(item, index) in dcComicsLinks" :key="index">
                <a :href="item.url">{{ item.title }}</a>
              </li>
            </ul>
            <h4>
              SHOP
            </h4>
            <ul>
              <li v-for="(item, index) in shopLinks" :key="index">
                <a :href="item.url">{{ item.title }}</a>
              </li>
            </ul>
          
          </div>
          <div>
            <h4>
              DC
            </h4>
            <ul>
              <li v-for="(item, index) in dcLinks" :key="index">
                <a :href="item.url">{{ item.title }}</a>
              </li>
            </ul>
            
          </div>
          <div>
            <h4>
              SITES
            </h4>
            <ul>
              <li v-for="(item, index) in sitelinks" :key="index">
                <a :href="item.url">{{ item.title }}</a>
              </li>
            </ul>
          </div>
        </div>
        
      </div>
    </div>
    <div class="bottom-footer">
      <div class="container">
        <div class="bottom-footer-cont">
          <div>
            <button class="btn-style">SIGN-UP NOW!</button>
          </div>
          <div class="bottom-links-cont">
            <ul>
              <li><a href="#">FOLLOW US</a></li>
              <li v-for="(social, index) in socialLinks" :key="index">
                <a :href="social.url">
                  <img :src="social.imgSrc" :alt="social.altText" />
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.container {
  max-width: 1300px;
  margin: 0 auto; 
}
.top-footer{
  background-image: url(../public/img/footer-bg.jpg);
  background-size: cover;
}
.top-footer .container{
  background-image: url(../public/img/dc-logo-bg.png);
  background-position: right;
 background-repeat: no-repeat;
}
.link-footer-top {
  padding-top: 50px;
  padding-bottom: 50px;
  display: flex;
  justify-content: space-between; 
  width: 33%; 
}
.link-footer-top div{
  flex-grow: 1;
}
.link-footer-top h4{
  color: white;
  padding: 20px 10px;
}
.link-footer-top ul {
  list-style: none;
}
.link-footer-top div ul li{
  padding-top: 5px;
  color:lightgrey;
}
.link-footer-top div ul li a{
  text-decoration: none;
  color:#607786;
}
.bottom-footer{
  background-color: #303030;

}

.bottom-footer-cont{
  display: flex;
  justify-content: space-between;
  align-items: center;
  min-height: 100px;
}
.btn-style{
  border: 2px solid #067AE6;
  padding: 13px;
  background-color:#303030 ;
  color: white;
  cursor: pointer;
  font-weight: bold;
}
.bottom-links-cont ul{
  display: flex;
  justify-content: space-around;
  list-style: none;
  text-decoration: none;
}

.bottom-links-cont ul li{
  padding: 5px;
  display: flex;
  align-items: center;
}

.bottom-links-cont ul li a{
  text-decoration: none;
  font-size: 1.28rem;
}

</style>
