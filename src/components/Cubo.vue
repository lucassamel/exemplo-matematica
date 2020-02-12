<template>
 
  <div class="card" style="max-width: 18rem;">
    <div class="card-header">Cubo</div>
      <div class="card-body">
        <h5 class="card-title">{{calcula_cubo()}}</h5>
        
      </div>
  </div>
  
</template>

<script>


export default {
  name: 'Cubo',
  props: {
    numero: Number,
    
  },
  data(){
    return { n : 4}
    }, methods :{
       calcula_cubo(){
         return this.n ** 3
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
