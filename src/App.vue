<script>
export default {
  data: () => ({
    contador: 500,
  }),
  methods: {
    saludar() {
      console.log("hola 10A | @");
    },
    incrementar() {
      this.contador++;
    },
    decrementar() {
      this.contador--;
    },
    resetear() {
      this.contador = 10;
    },
  },
};
</script>

<template>
  <nav class="navbar navbar-light bg-light">
    <span class="navbar-brand mb-0 h1"></span>
    <h1>Juan Carlos Cervantes Romero 10 A</h1>
  </nav>
  <img src="./assets/logo.png" alt="logo VUE" width="125" height="125" />
  <div class="container">
    <small><h1>HOLA VUE.JS 3</h1></small>
    <hr />
    <h2>Contandor {{ contador }}</h2>
    <button v-on:click="saludar">Saludar</button>
    <button @click="saludar()">Saludar</button>
    <button @click="incrementar">+1</button>
    <button @click="decrementar">-1</button>
    <button @click="resetear">Reset</button>
  </div>
</template>

<style scoped>
.container {
  text-align: center;
}
small {
  color: #666;
}

h1 {
  font-weight: border;
}

h2 {
  font-size: 2.5rem;
}

button {
  cursor: pointer;
  font-size: 1.5rem;
  margin: 3px, 8px;
}
</style>