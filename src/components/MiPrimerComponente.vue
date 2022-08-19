<template>
<div class="main">
  <h1>Este es mi primer componente en vue 👻</h1>
  <div>
    <h3>{{mi_primer_variable}}</h3>
    <h4>{{otra_variable}}</h4>
    <h5>{{variableEstatica}}</h5>
    <p>Aqui estoy utilizando una variable computada para hacer que {{otra_variable}} se convierta en {{double}}</p>
    <p>Aqui estoy utilizando variables computadas anidadas para que a {{otra_variable}} sea {{plusOne}} y al final se convierta en {{triple}}</p>
  </div>
</div>
</template>

<script>
const variableEstatica = 'Esto es una variable estatica 🤫'

export default {
  name: 'MiComponente',
  data: () => ({
    mi_primer_variable: 'Esta es mi primer variable 😃',
    otra_variable: 20,
    variableEstatica
  }),
  computed: {
    double () {
      return this.otra_variable * 2
    },
    plusOne () {
      return this.otra_variable + 1
    },
    triple () {
      return this.plusOne * 3
    }
  }
}
</script>

<style scoped>
h1 {
  color: rgb(50,150,150);
}
</style>
