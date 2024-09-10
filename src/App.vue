<script>
//1- Importazione del componenente necessario che voglio aggiungere qua


export default {
  data() {
    return {

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
  <header>
    <div class="container">
      <div class="header-content">
        <div class="logo-cont"><img src="../public/img/dc-logo.png" alt="dc-logo"></div>
        <div class="link-header-cont">
          <ul>
            <li><a href="#">CHARACTERS</a></li>
            <li class="active"><a href="#">COMICS</a></li>
            <li><a href="#">MOVIES</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">GAMES</a></li>
            <li><a href="#">COLLECTIBLES</a></li>
            <li><a href="#">VIDEOS</a></li>
            <li><a href="#">FANS</a></li>
            <li><a href="#">NEWS</a></li>
            <li><a href="#">SHOP</a></li>
          </ul>
        </div>
      </div>
    </div>
  </header>
  <main>
    <div class="container">
      <div>
        <p>-- MIAN CONTENT GOES HERE --</p>
      </div>
    </div>
  </main>
  <div class="main-links">
    <div class="container">
      <div class="ads-container">
        <ul>
          <li>
            <div><img src="../public/img/buy-comics-digital-comics.png" alt=""></div>
            <div><a href="#">DIGITAL COMICS</a></div>
          </li>
          <li>
            <div><img src="../public/img/buy-comics-merchandise.png" alt=""></div>
            <div><a href="#">DC MERCHANDISE</a></div>
          </li>
          <li>
            <div><img src="../public/img/buy-comics-shop-locator.png" alt=""></div>
            <div><a href="#">SUBSCRIPTION</a></div>
          </li>
          <li>
            <div><img src="../public/img/buy-comics-subscriptions.png" alt=""></div>
            <div><a href="#">COMIC SHOP LOCATOR</a></div>
          </li>
          <li>
            <div><img src="../public/img/buy-dc-power-visa.svg" alt=""></div>
            <div><a href="#">DC POWER VISA</a></div>
          </li>
        </ul>
      </div>
    </div>
  </div>
  <footer>
    <div class="top-footer">
      <div class="container">
        <div class="link-footer-top">
          <div>
            <h4>
              DC COMICS
            </h4>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h4>
              SHOP
            </h4>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          
          </div>
          <div>
            <h4>
              DC
            </h4>
            <ul>
            <li><a href="#">Terms Of Use</a></li>
            <li><a href="#">Privacy Policy (New)</a></li>
            <li><a href="#">Ad Choices</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Jobs</a></li>
            <li><a href="#">Subscriptions</a></li>
            <li><a href="#">Talent Workshops</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact Us</a></li>
            </ul>
            
          </div>
          <div>
            <h4>
              SITES
            </h4>
            <ul>
              <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>
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
              <li><a href="#"><img src="../public/img/footer-facebook.png" alt=""></a></li>
              <li><a href="#"></a><img src="../public/img/footer-periscope.png" alt=""></li>
              <li><a href="#"></a><img src="../public/img/footer-pinterest.png" alt=""></li>
              <li><a href="#"></a><img src="../public/img/footer-youtube.png" alt=""></li>
              <li><a href="#"></a><img src="../public/img/footer-twitter.png" alt=""></li>
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
  position: relative;
}

header {
  background-color: #FFFFFF;
  height: 100px;
}

.header-content {
  width: 100%;
  display: flex;
  align-content: center;
  justify-content: space-between;
}

.logo-cont img {
  max-width: 100%;
  max-height: 80%;
}

.link-header-cont {
  display: flex;
  align-items: center;
}

.link-header-cont ul {
  display: flex;
  flex-wrap: wrap;
  list-style: none;
  text-decoration: none;

}

.link-header-cont ul li {
  padding: 10px;
}

.link-header-cont ul li a {
  text-decoration: none;
  color: black;
}

.link-header-cont ul li.active a {
  color: blue;
}

main {
  min-height: 150px;
  background-color: #1C1C1C;
}

.container div p {
  color: white;
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
