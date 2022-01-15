<template>
<v-app>
<v-app-bar app color="primary" dark>
  <v-app-bar-nav-icon @click="drawer=!drawer"
                      class="white--text">
  </v-app-bar-nav-icon>
  <v-app-bar-title class="white--text">
    Catchup
  </v-app-bar-title>
</v-app-bar>
<v-main>
  <v-content>
    <v-container fluid>
    <!--   llama al componente main-contetn -->
<main-content :articles ="articles">

</main-content>
    </v-container>
  </v-content>
  <v-footer class="secondary" app>
    Made with <v-icon class="red--text">mdi-heart</v-icon>
    using <a class="white--text"></a>
  </v-footer>
</v-main>
</v-app>
  
</template>

<script>
import axios from "axios";
import MainContent from './components/main-content.vue';
export default {
  name: 'App',

  components: {
    MainContent
   
  },

   data:()=>({
drawer:false,
apiKey:'',
articles : [],
errors : [],
   }),
     created(){
axios.get( 'https://newsapi.org/v2/top-headlines?country=us&apiKey=075640c99ce94ef3aafdb7f1a3b09f4f')
.then(response => {
/* response.data.articles es proque dentro del json va contener articles;*/ 
 /* objeto coleccion articles*/
 this.articles=response.data.articles;
 console.log('data:');
 console.log(response.data.articles)
})
     }
    };
 </script>
