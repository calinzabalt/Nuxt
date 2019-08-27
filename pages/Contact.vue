<template>
<div class="contact">
<Intro2 />
 <v-container>
    <h1>Metode de contact:</h1>
    <p>0740 691 940 <br>
       Websolvercalin@gmail.com
    </p>      
   <Cform />
   </v-container>
   </div>
</template>

<script>
import Intro2 from '~/components/Intro2.vue'
import Cform from '~/components/Cform.vue'

export default {
  components: {
    Intro2,
    Cform
  },
  data () {
  return {
    title: 'Contact'
  }
},
head () {
  return {
    title: this.title,
    meta: [
      { hid: 'description', name: 'description',content: 'Pagina de contact' }
     ]
    }
  }
}


</script>

<style scoped>
h1{
  color: #293347;
  text-align:center;
}
p{
  color: #293347;
  text-align:center;
  font-size: 20px;
}
</style>

