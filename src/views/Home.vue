<template>
  <div class="home">
        <div id="nav">
      <router-link to="/">Tahap 1</router-link> |
      <router-link to="/about">Tahap 2</router-link> |
      <router-link to="/tahap-3">Tahap 3</router-link>
    </div>
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>
