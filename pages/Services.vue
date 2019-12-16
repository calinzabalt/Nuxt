<template>
 <v-container>
   <h1>Latest Projects</h1>
   <Carousel />
   <Table />
   <div class="services">
   <h1>Packages & Pricing</h1>
   </div>
   <p>From hosting and finding the right domain, to building websites and maintaining them everyday.</p>
   <Pack />
   <Mentenanta />
    </v-container>
</template>

<script>
import Pack from '~/components/Pack.vue'
import Carousel from '~/components/Carousel.vue'
import Table from '~/components/Table.vue'
import Mentenanta from '~/components/Mentenanta.vue'

export default {
  components: {
    Pack,
    Carousel,
    Table,
    Mentenanta
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
.services {
  margin-top: 20px
}
p{
  color: #293347;
  margin: 10px;
  font-size: 22px;
  font-family: "eurostile",sans-serif;
  font-weight: 300;
  text-align: center;
}
h1{
  padding-top: 16px;
  color: #293347;
  text-align:center;
}
</style>
