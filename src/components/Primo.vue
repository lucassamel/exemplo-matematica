<template>
  <div class="card" style="max-width: 18rem;">
    <div class="card-header">Primo</div>
      <div class="card-body">
        <h5 class="card-title">{{calcula_primo()}}</h5>
        
      </div>
  </div>
  
</template>

<script>


export default {
  name: 'Primo',
  props: {
    numero: Number,
    
  },
  data(){
    return { n : 4}
    }, methods :{
       calcula_primo(){
        let resultado = 'Este numero é um numero primo'
        let i = 2;
        for(i=2; i<this.n-1; i++){
          if((this.n % i) == 0){
           resultado ='Este não é um numero primo'
      }
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
