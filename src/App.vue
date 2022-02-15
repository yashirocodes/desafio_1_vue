<template>
  <div>
    <div class="container">
      <table class="table">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Nombre</th>
      <th scope="col">Rut</th>
      <th scope="col">Telefono</th>
      <th scope="col">Mes de nacimiento</th>
      <th scope="col">Edad</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="usuario in usuarios" :key="usuario">
      <th scope="row">{{usuario.id}}</th>
      <td>{{usuario.nombre}}</td>
      <td>{{usuario.rut}}</td>
      <td>{{usuario.telefono}}</td>
      <td>{{usuario.nacimiento}}</td>
      <td>{{usuario.edad}}</td>
    </tr>
  </tbody>
</table>
    </div>
  </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.min.css"
export default {
  name: 'App',
  data(){
    return{
      usuarios: [{
        id:1,
        nombre:"jorge",
        rut: 11111,
        telefono: 555999555,
        nacimiento: "abril",
        edad: 20,

      },
      {
        id:2,
        nombre:"manuel",
        rut: 2222,
        telefono: 444555666,
        nacimiento: "mayo",
        edad: 25,
      },
      {
        id:3,
        nombre:"jose",
        rut: 3333,
        telefono:888555222,
        nacimiento: "noviembre",
        edad: 40,
      }],
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
