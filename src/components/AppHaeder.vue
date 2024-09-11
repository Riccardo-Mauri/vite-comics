<script>
//1- Importazione del componenente necessario che voglio aggiungere qua


export default {
  data() {
    return {
      headerlinks:[
        {
          label: 'CHARACTERS',
          url: '#',
          active: false
        },
        {
          label: 'COMICS',
          url: '#',
          active: true
        },
        {
          label: 'MOVIES',
          url: '#',
          active: false
        },
        {
          label: 'TV',
          url: '#',
          active: false
        },
        {
          label: 'GAMES',
          url: '#',
          active: false
        },
        {
          label: 'COLLECTIBLES',
          url: '#',
          active: false
        },
        {
          label: 'VIDEOS',
          url: '#',
          active: false
        },
        {
          label: 'FANS',
          url: '#',
          active: false
        },
        {
          label: 'NEWS',
          url: '#',
          active: false
        },
        {
          label: 'SHOP',
          url: '#',
          active: false
        },
        
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
  <header>
    <div class="container">
      <div class="header-content">
        <div class="logo-cont"><img src="/img/dc-logo.png" alt="dc-logo"></div>
        <div class="link-header-cont">
          <ul>
            <li v-for="(link, index) in headerlinks" :key="index">
              <a :href="link.url" :class="{
                'active': link.active}">
                {{ link.label }}
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </header>
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

.active{
  color: blue;
}
</style>
