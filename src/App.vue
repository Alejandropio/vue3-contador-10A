<script>
  export default{
    data: () => ({
        contador:500,
    }),
    methods:{
      saludar(){
        console.log("Hola 10A");
      },
      incrementar(){
        this.contador++;
      },
      decrementar(){
        this.contador--;
      },
      resetear(){
        this.contador = 500;
      },

    }
  };
</script>

<template>
  <nav class="navbar navbar-dark bg-dark">
    <a class="navbar-brand" href="#">Alejandro Zepeda Pioquinto "10 A "</a>
  </nav>
  
  <img src="./assets/logo.svg" alt="Logo VUE" width="125" height="125">
  <div class="container">
    
    <small>
      <h1>hola desde VUE.JS 3</h1>
    </small>
    <hr>
    <h2> contador {{ contador }}</h2>
    <button v-on:click="incrementar()">+1</button>
    <button v-on:click="decrementar()">-1</button>
    <button @click="resetear()">Reset</button>
  </div>
</template>

<style scoped >
 .container {
  text-align: center;
  }
  small {
    color:#666;
  }
  h1{
    font-weight: bolder;
  }
  h2 {
    font: size 2.5rem;
    margin:0px;
  }
</style>