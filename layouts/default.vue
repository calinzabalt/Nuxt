<template>
  <v-app dark>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar
      :clipped-left="clipped"
      fixed
      app
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <nuxt-link to="/#">
      <v-img
      src="images/logo.png"
      max-height="50"
      max-width="50"
      contain
      ></v-img>
      </nuxt-link>
      <v-spacer />
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn aria-label="Home" text to="/#">Home</v-btn>
        <v-btn aria-label="Services" text to="/Services">Services</v-btn>
        <v-btn aria-label="Contact" text to="/Contact">Contact</v-btn>
       
      </v-toolbar-items>  
    </v-app-bar>

    <v-content>
      <v-container fluid style="margin: 0px; padding: 0px; width: 100%">
        <nuxt />
      </v-container>
    </v-content>
   
    <v-footer>
      <no-ssr><cookie-law theme="dark-lime"></cookie-law></no-ssr>
      <v-layout justify-center row wrap>
      <v-flex xs12 sm4>
      <div class="social">
        <p>Social media links:</p>
        <v-btn aria-label="facebook" type='button' href="https://www.linkedin.com/in/cozma-viorel-calin-947658145/" target="blank" large icon class="light-blue darken-4">
            <v-icon medium color="white">mdi-linkedin</v-icon>
        </v-btn>
        <v-btn aria-label="linkedn" type='button' href="https://www.facebook.com/CozmaViorelCalinPFA/" target="blank" large icon class="light-blue darken-3">
            <v-icon medium color="white">mdi-facebook</v-icon>
        </v-btn>
        <v-btn aria-label="youtube" type='button' href="https://www.youtube.com/channel/UC2CNVDGd1odpr7UqsiIM68g?view_as=subscriber" target="blank" large icon class="deep-orange darken-4">
            <v-icon medium color="white">mdi-youtube</v-icon>
        </v-btn>
        <v-btn aria-label="instagram" type='button' href="https://twitter.com/Cozmaviorelcal1" target="blank" large icon class="light-blue darken-2">
            <v-icon medium color="white">mdi-twitter</v-icon>
        </v-btn>
      </div>
    </v-flex>    
    <v-flex xs12 sm4>
      <div class="available">
      <p>Cozma Viorel Calin (PFA)</p>
      <p>websolvercalin@gmail.com</p>
      <p>Phone: 0740 691 940</p>
       <v-btn aria-label="contact" type='button' to="/contact" id="v-parallax" color="blue" large>Contact</v-btn> 
        
    </div>
    </v-flex> 
     <v-flex xs12 sm4>
      <div class="links">
        <p>Useful Links:</p>
         <v-btn aria-label="terms" text to="/terms"><h4>Terms & Conditions</h4></v-btn><br/>
         <v-btn aria-label="privacy" text to="/terms"><h4>Privacy policy</h4></v-btn>
        </div>
    </v-flex>  
    <div class="copy">
   <h5>&copy;2019 — All rights reserved></h5>
    </div>
    </v-layout>    
    </v-footer>
  </v-app>
</template>

<style scoped>
footer { 
  margin-top: 30px;
  justify-content: center;
  text-align: center;
}
.v-footer p{
  font-size: 20px;
  margin: 0;
  padding: 0;
  font-weight: 400;
}

.copy{
  margin-bottom: 10px;
}

.social{
  margin-top: 10px;
  padding: 20px;
}

.links{
  margin-top: 10px;
  padding: 20px;
}

.available{
  padding: 20px;
}
</style>

<script>
import CookieLaw from 'vue-cookie-law'

export default {
  components:  {
    CookieLaw
},

  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-home',
          title: 'Home',
          to: '/'
        },
        {
          icon: 'mdi-briefcase',
          title: 'Services',
          to: '/Services'
        },
        {
          icon: 'mdi-contact-phone',
          title: 'Contact',
          to: '/Contact'
        },
         {
          icon: 'mdi-information',
          title: 'Terms & Conditions',
          to: '/Terms'
        },
        {
          icon: 'mdi-information-outline',
          title: 'Privacy policy',
          to: '/Terms'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Websolver'
    }
  }
}
</script>
