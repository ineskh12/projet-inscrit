<template>
 
  <table border >
  <tr>
    <th>Prénom</th>
    <th>Nom</th>
    <th>Agz</th>
  </tr>

 <tr v-for="(personne,index) in liste" :key="index">
   <td>{{ personne.prenom }}</td>
   <td>{{ personne.nom }}</td>
   <td>{{ personne.age }}</td>
 </tr>
</table>

</template>

<script>
export default {
  name: 'InscritPage',
  props: ['liste']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
th {
  background: lightgray;
  font-size: 140%;
}
td{
  width: 10rem;
  text-align: center;
}
</style>
