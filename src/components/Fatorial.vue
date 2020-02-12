<template>
  <div class="card" style="max-width: 18rem;">
    <div class="card-header">Fatorial</div>
      <div class="card-body">
        <h5 class="card-title">{{calcula_fatorial()}}</h5>
        
      </div>
  </div>
  
</template>

<script>


export default {
  name: 'Fatorial',
  props: {
    numero: Number,
    
  },
  data(){
    return { n : 4}
    }, methods :{
       calcula_fatorial(){
         let resultado = 1 
         let i = 1;
         for(i=1; i<this.n+1; i++){
           resultado *= i
      }
     return resultado
    }
    } 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.card {
  display: flex;
  padding: 24px;
  justify-content: space-between;
  margin: auto;
}
</style>
