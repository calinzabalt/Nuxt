<template>
<v-container>
  <v-layout row wrap>
    <v-flex xs12>
    <v-carousel height="auto">
    <v-carousel-item 
      v-for="(item,i) in items"
      :key="i"
      :src="item.src">
      <div class="title">
          {{ item.title}}
      </div>  
    </v-carousel-item>
  </v-carousel>
    </v-flex>
  </v-layout>  
</v-container>  
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: '/images/pipemax.png', title: 'Servicii profesionale de Ozonizare si Decarbonizare (Pipemax.ro)'
          },
          {
            src: '/images/vremea1.png', title: 'Află vremea din orasul tau'
          },
          {
            src: '/images/via.png', title: 'Progreseaza prin inovatie (viaengineering-development.com)'
          },
          {
            src: '/images/books.png', title: 'Aceasta este o aplicație unde puteți căuta cărțile preferate.'
          },
          {
            src: '/images/reminder1.png', title: 'Construiește-ți lista online cu reminder'
          }
        ]
      }
    }
  }
</script>

<style scoped>

.title{
  position: absolute;
  margin-left: auto;
  margin-right: auto;
  left: 0;
  right: 0;
  bottom: 50px;
  background-color: rgba(0, 0, 0, 0.5);
  color: white;
  font-size: 2em;
  padding: 10px;
}

</style>