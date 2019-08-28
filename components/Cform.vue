<template>
    <v-container>
         <v-layout>
        <v-flex>
        <v-form name="contact" method="POST" data-netlify="true">
          <v-card>
           <v-card-text>
            <v-row>
                <v-text-field
                    type="text"
                    name="name"
                    v-model="firstname"
                    :rules="nameRules"
                    :counter="30"
                    label="Nume"
                    required
                ></v-text-field>
                          
                <v-text-field
                    type="email"
                    name="email"
                    v-model="email"
                    :rules="emailRules"
                    label="E-mail"
                    required
                ></v-text-field>
                 </v-row>
                <v-row>
                <v-textarea
                    name="message"
                    counter
                    :rules="MesajRules"
                    label="Mesaj"
                    :value="Mesaj"
                 ></v-textarea>
                </v-row>
             <v-btn color="primary" type="submit">Trimite</v-btn>
                 </v-card-text>
                </v-card>
            </v-form>
       </v-flex>
    </v-layout>
  
    </v-container>
</template>

<script>
export default {
    data: () => ({
      valid: false,
      firstname: '',
      lastname: '',
      nameRules: [
        v => !!v || 'Numele este obligatoriu',
        v => v.length <= 30 || 'Name must be less than 30 characters',
      ],
      email: '',
      emailRules: [
        v => !!v || 'E-mail este obligatoriu',
        v => /.+@.+/.test(v) || 'E-mail trebuie sa fie valid',
      ],
      Mesaj: '',
      MesajRules: [
        v => v.length <= 1500 || 'Mesaj-ul trebuie sa fie mai scurt de 1500 de caractere',
      ]
    }),
  }
</script>

<style scoped>
.v-text-field{
    margin: 10px;
}
.v-card{
    max-width: 800px;
    text-align: center;
    margin-left: auto;
    margin-right: auto;
}
</style>

