<template>
  <div class="card" style="max-width: 18rem;">
    <div class="card-header">Quadrado</div>
      <div class="card-body">
        <h5 class="card-title">{{calcula_quadrado()}}</h5>
        
      </div>
  </div>
  
</template>

<script>


export default {
  name: 'Quadrado',
  props: {
    msg: String,
    
  },
  data(){
    return { n : 4}
    }, methods :{
       calcula_quadrado(){
         return this.n ** 2
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
