<script setup>
// import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <HelloWorld msg="Welcome to Kei's Project Portal!" />
  </header>

  <nav>
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/test">Test</RouterLink>
  </nav>

  <RouterView />
</template>

<style scoped>

</style>
