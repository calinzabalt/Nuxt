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
            src: '/images/pipemax.png', title: 'Professional Ozonation and Decarbonisation Services (Pipemax.ro)'
          },
          {
            src: '/images/vremea1.png', title: 'Find out the weather in your city'
          },
          {
            src: '/images/via.png', title: 'Progress through innovation (viaengineering-development.com)'
          },
          {
            src: '/images/books.png', title: 'This is an application where you can search for your favorite books.'
          },
          {
            src: '/images/reminder1.png', title: 'Build your online list with reminder'
          }
        ]
      }
    }
  }
</script>

<style scoped>
.v-carousel {
 border: 4px solid #333745;
 border-radius: 0px 20px 0px 0px;
 margin-bottom: 10px;
}

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