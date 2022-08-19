<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Hi! This is my first proyect with vue 👋"/>
    <MiComponente/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import MiComponente from '@/components/MiPrimerComponente.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    MiComponente
  }
}
</script>
