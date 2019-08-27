<template>
 <v-container>
   <h1>Servicii Web</h1>
   <p>De la găzduire și găsirea domeniului potrivit, până la implementarea și întreținerea site-ului web zilnic.</p>
   <Pack />
   <Carousel />
   <Table />
  </v-container>
</template>

<script>
import Pack from '~/components/Pack.vue'
import Carousel from '~/components/Carousel.vue'
import Table from '~/components/Table.vue'

export default {
  components: {
    Pack,
    Carousel,
    Table
  },
data () {
  return {
    title: 'Servicii'
  }
},
head () {
  return {
    title: this.title,
    meta: [
      { hid: 'description', name: 'description',content: 'Servicii web complete' }
     ]
    }
  }
}
</script>

<style scoped>
p{
  padding-bottom: 10px;
  color: #293347;
  margin: 10px;
  font-size: 22px;
  font-family: "eurostile",sans-serif;
  font-weight: 300;
  text-align: center;
}
h1{
  color: #293347;
  text-align:center;
}
</style>
