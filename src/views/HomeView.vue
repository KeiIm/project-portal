<script setup>
import HelloWorld from '../components/HelloWorld.vue'
import Card from 'primevue/card'
</script>

<template>
  <header>
    <HelloWorld msg="Kei's Project Portal" />
  </header>

  <h2>Choose a Project:</h2>

  <section class="container">
    <Card class="card">
      <template #header>
        <RouterLink to="/navi"><img src="/images/reddit-card.png"></RouterLink>
      </template>
      <template #title>
        <RouterLink to="/navi">Naveena's Homepage</RouterLink>
      </template>
      <template #content>This is a test project.</template>
      <!-- <template #footer></template> -->
    </Card>
    <Card class="card">
      <template #header>
        <RouterLink to="/test"><img src="/images/reddit-card.png"></RouterLink>
      </template>
      <template #title>
        <RouterLink to="/test">Test Project</RouterLink>
      </template>
      <template #content>This is a test project.</template>
    </Card>
    <Card class="card"></Card>
    <Card class="card"></Card>
    <Card class="card"></Card>
    <Card class="card"></Card>
  </section>

</template>

<style scoped>
*,
*:before,
*:after {
  box-sizing: border-box;
}

header {
  margin-top: 2rem;
}

.container {
  width: 100%;
  flex: auto
}

.card {
  max-width: 100%;
  width: 300px;
  height: 600px;
  float: left;
  margin: 0.4rem;
  border-radius: 15px;
}

.card a {
  text-decoration: none;
  color: white
}
</style>