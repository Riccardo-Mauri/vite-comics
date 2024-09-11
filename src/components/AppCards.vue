<script>
//1- Importazione del componenente necessario che voglio aggiungere qua


export default {
  props:{
    thumb: String, // è l'immagine o copertina del fumetto/film
    price: String, //è il prezzo del film/fumetto
    series: String, //è il nome del film/fumetto
    type: String, // il tipo o categoria ( ad esempio "comic book")
  },
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
 <div class="comic-item">
  <div class="comic-ite-img-cont"><img :src="thumb" :alt="series"> </div>
  <div class="comic-title"><h3>{{ series }}</h3></div>
 </div>
</template>

<style scoped>
  .comic-item{
    margin: 0 10px;
    padding-top: 30px;
    width:calc((100% / 6) - 20px);
    height: 200px;
    display: flex;
    flex-direction: column;
  }
  .comic-ite-img-cont{
    flex-grow: 2;
    display: flex;
    justify-content: center;
    align-items: center;
    max-height: 170px;
  }
  .comic-ite-img-cont img {
    width: 100%;
    height: 100%; 
    object-fit: cover;
  }
  .comic-title{
    flex-grow: 1; 
    text-align: center; 
    font-size: 12px;
    color: white; 
  }
</style>
