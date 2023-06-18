<script>
export default {
  data: () =>({
    contador:10,
  }),
  methods: {
saludar(){
console.log("Hola "+ this.contador)
},
incrementar(){
  this.contador++;
},
restar(){
  this.contador--;
},
resetear(){
this.contador=10;
},
  }

};

</script>

<template>

<div>
  <img src="./assets/logo.svg" alt="logo vue" width="125">
  <h1>Hola Mundo desde Vue.js 3</h1>

  <hr />
  <h2>Contador : {{ contador }}</h2>
  <button @click="incrementar">+1</button>
  <button @click="restar">-1</button>
  <button @click="resetear">Reset</button>

</div>
  
</template>

<style scoped>
.container{
  text-align: center;
  background-color: #ddd;
}
h1{
  color: red;
}
h2{
  font-size: 2.5rem;
}
button{
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 6px;
}

</style>