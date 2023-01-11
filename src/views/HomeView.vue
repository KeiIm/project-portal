<script setup>
import HelloWorld from '../components/HelloWorld.vue'
</script>

<template>
  <main>
    <header>
      <HelloWorld msg="Welcome to Kei's Project Portal!" />
    </header>
    <h2>List of Projects:</h2>
    <ul>
      <li>
        <RouterLink to="/test">Test</RouterLink>
      </li>
    </ul>
  </main>
</template>
