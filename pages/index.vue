<template>
<div>
 <Intro />
 <Presentation />
 <About />
</div>
</template>

<script>
import Intro from '~/components/Intro.vue'
import About from '~/components/About.vue'
import Presentation from '~/components/Presentation.vue'

export default {
  components: {
    Intro,
    About,
    Presentation
  },

data () {
  return {
    title: 'Welcome!'
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
