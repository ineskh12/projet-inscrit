<template>
  

  <h1>List des Inscrit</h1>
  <InscritPage :liste="personnes"> </InscritPage>
</template>

<script>
import InscritPage from './components/InscritPage.vue'

export default {
  name: 'App',
  components: {
    InscritPage
  }, 
  data(){
    return{
       personnes:[
        {prenom:"Ines",nom:"Khelifi",age:29}
       ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}


</style>
