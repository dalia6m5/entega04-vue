<template>
  <div id="app">
    
   
    <SingUp/>
    <LogIn/>
    <ListaProd/>
    <ProdDetalle/>
    <CarritoProd/>
  </div>
</template>

<script>
/* import HelloWorld from './components/HelloWorld.vue' */
import SingUp from './components/SingUp.vue'
import LogIn from './components/LogIn.vue'
import ListaProd from './components/ListaProd.vue'
import CarritoProd from './components/CarritoProd.vue'
import ProdDetalle from './components/ProdDetalle.vue'



export default {
  name: 'App',
  components: {
   
    SingUp,
    LogIn,
    ListaProd,
    CarritoProd,
    ProdDetalle,

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
