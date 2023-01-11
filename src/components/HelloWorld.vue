<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<!-- This is a replaceable component -->

<template>

  <h1>{{ msg }}</h1>

</template>

<style scoped>

</style>
