<template>
<div>
 <Intro />
 <About />
 <Cards />
 <Plan />
 </div>
</template>

<script>
import Intro from '~/components/Intro.vue'
import About from '~/components/About.vue'
import Cards from '~/components/Cards.vue'
import Plan  from '~/components/Plan.vue'

export default {
  components: {
    Intro,
    About,
    Cards,
    Plan
  },

data () {
  return {
    title: 'Bine ai venit!'
  }
},
head () {
  return {
    title: this.title,
    meta: [
      { hid: 'description', name: 'description',content: 'Bine ai venit pe Website-ul nostru' }
     ]
    }
  }
}
</script>
