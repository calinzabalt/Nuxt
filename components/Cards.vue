<template>
  <v-container grid-list-xl text-xs-center>
    <v-layout row wrap>
      <v-flex xs12 md4 sm4>
        <v-card>
        <v-img
          src="/images/What.png"
          aspect-ratio="1.2"
        ></v-img>

        <v-card-title primary-title>
          <div>
            <p><strong>Ce facem noi ?</strong></p>
            <p>Noi construim website-uri unice si profesionale pentru orice tip de companie,
               startap-uri si freelancers (liberi independenti)
            </p>
          </div>
        </v-card-title>

        <v-card-actions>
          <v-btn dark type='button' aria-label="Servici" to="/Services" id="top" class="mx-1" color="#039BE5"><strong>Servicii</strong></v-btn>
        </v-card-actions>
      </v-card>
        </v-flex>

      <v-flex xs12 md4 sm4>
        <v-card>
        <v-img
          src="/images/how.png"
          aspect-ratio="1.2"
        ></v-img>

        <v-card-title primary-title>
          <div>
            <p><strong>Ce tehnologi folosim ?</strong></p> 
            <p>Noi folosim tehnologi precum React.js, Vue.js, Netlify,
               Wordpress, Drupal pentru a satisface nevoile clientilor.
            </p>   
          </div>
        </v-card-title>

        <v-card-actions>
          <v-btn dark type='button' aria-label="Servici" id="top" to="/Services" class="mx-1" color="#039BE5"><strong>Servicii</strong></v-btn>
        </v-card-actions>
      </v-card>
      </v-flex>

      <v-flex xs12 md4 sm4>
        <v-card>
        <v-img
          src="/images/why.png"
          aspect-ratio="1.2"
        ></v-img>

        <v-card-title primary-title>
          <div>
            <p><strong>De ce ?</strong></p>
            <p>Noi construim website-uri deoarece ne place sa ajutam
               oameni sa isi realizeze obiectivele si visele.
            </p>   
          </div>
        </v-card-title>

        <v-card-actions>
         <v-btn dark type='button' aria-label="Servici" id="top" to="/Services" class="mx-1" color="#039BE5"><strong>Servicii</strong></v-btn>
        </v-card-actions>
      </v-card>
        
      </v-flex>
    </v-layout>
  </v-container>
</template>

<style scoped>
p {
  text-align: center;
}
</style>