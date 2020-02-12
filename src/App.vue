<template>
  <div id="app">

    <div id="box">
      <Quadrado :numero="5" />
      <Cubo/>
    </div>       
    
    <div id="box">
     <Primo/>
      <Fatorial/>
    </div>
   
  </div>
</template>

<script>


import Cubo from './components/Cubo.vue'
import Quadrado from './components/Quadrado.vue'
import Primo from './components/Primo.vue'
import Fatorial from './components/Fatorial.vue'



export default {
  name: 'app',
  components: {
    Cubo,
    Quadrado,
    Primo,
    Fatorial
  }, data() {
    return {
      horas : new Date(),
      mensagem : "Lucas",
      n : 5
    }
  }, methods : {
    
    
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  display: flex;
}

#box{
  vertical-align: baseline;
  display: flex;
  padding: 24px;
  justify-content: space-between;
  margin: auto;
}
</style>
