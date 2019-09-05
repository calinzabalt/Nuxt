<template>
    <v-container grid-list-xl text-xs-center>
         <v-card><h1>Proces</h1> 
        <v-layout row wrap>
            <v-flex xs12 md4 sm4>
            <v-img
                src="/images/1.png"
                aspect-ratio="1.8"
            ></v-img>
                <v-card-title primary-title>
                    <div class="text">
                        <h3>"Analizare"</h3>
                        <p>  Scopul Website-ului, 
                             Obiectivele, 
                             Publicul Tinta 
                        </p>
                   </div>
                </v-card-title>
            </v-flex>
            <v-flex xs12 md4 sm4>
                  <v-img
                    src="/images/2.png"
                    aspect-ratio="1.8"
                  ></v-img>
                <v-card-title primary-title>
                    <div class="text">
                        <h3>"Plan"</h3>
                        <p> Strucura Website-ului, 
                            Tehnologiile utilizate
                        </p>
                   </div>
                </v-card-title>
            </v-flex>
            <v-flex xs12 md4 sm4>
                  <v-img
                    src="/images/3.png"
                    aspect-ratio="1.8"
                  ></v-img>
                <v-card-title primary-title>
                    <div class="text">
                        <h3>"Continut"</h3>
                        <p> Imagini, Video-uri, Text, Optimizare SEO
                        </p>
                   </div>
                </v-card-title>
            </v-flex>
        </v-layout>
        <v-layout row wrap>
             <v-flex xs12 md4 sm4>
                   <v-img
                    src="/images/4.png"
                    aspect-ratio="1.8"
                  ></v-img>
                <v-card-title primary-title>
                    <div class="text">
                        <h3>"Dezvoltare"</h3>
                        <p>  Html & Css, 
                             Javascript,
                             React.js, Vue.js,
                             Netlify,
                             Wordpress.
                        </p>
                   </div>
                </v-card-title>
            </v-flex>
            <v-flex xs12 md4 sm4>
                  <v-img
                    src="/images/5.png"
                    aspect-ratio="1.8"
                  ></v-img>
                <v-card-title primary-title>
                    <div class="text">
                        <h3>"Testare"</h3>
                        <p> Testare tehnica, Compatibilitate browserului, Isi indeplineste scopul ?
                        </p>
                   </div>
                </v-card-title>
            </v-flex>
             <v-flex xs12 md4 sm4>
                   <v-img
                    src="/images/6.png"
                    aspect-ratio="1.8"
                  ></v-img>
                <v-card-title primary-title>
                    <div class="text">
                        <h3>"Implementare"</h3>
                        <p>Monitorizare, Corectarea erorilor, Intretinere.
                        </p>
                   </div>
                </v-card-title>
            </v-flex>
            
        </v-layout>
        </v-card>
    </v-container>
</template>

<style scoped>
.text{
    margin-left: auto;
    margin-right: auto;
}
p{
    text-align: center;
    font-size: 20px;
    color: #293347;
}
h1{
    text-align: center;
    margin-bottom: 20px;
    color: #293347;
}
h3{
    text-align: center;
    color: #293347;
}
</style>