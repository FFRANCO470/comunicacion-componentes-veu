<template>
  <div id="app">
    <h2>padre</h2>
    <h1>{{saludo}}</h1>
    <hr>
    <hijo1 :recibiendo="enviando"/>
    <hijo2 @recibirHijo = "saludo=$event"/>
    <hijo3/>
    <hijo4/>

  </div>
</template>
<script>
import hijo1 from './components/hijo1'
import hijo2 from './components/hijo2'
import hijo3 from './components/hijo3'
import hijo4 from './components/hijo4'
export default {
  name: 'App',
  components: {
    hijo1,
    hijo2,
    hijo3,
    hijo4
  },
  data(){
    return{
      enviando: 'info del padre al hijo',
      saludo:''
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
