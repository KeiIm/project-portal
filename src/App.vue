<script setup>
import Menubar from 'primevue/menubar'
</script >

<template>
  <Menubar :model="items" class="menu-bar" />
  <!-- <button @click="$router.back()">Go Back</button> -->
  <RouterView />
</template>

<script>
export default {
  data() {
    return {
      items: [
        { label: 'Home', to: '/' },
        {
          label: 'Projects',
          items: [
            {
              label: "Naveena's Homepage",
              to: '/navi',

            },
            { separator: true },
            {
              label: 'Test',
              to: '/test',
              // icon: 'pi pi-fw pi-file',
            },
          ]
        },
      ]
    }
  }
}
</script>

<style>
.menu-bar {
  margin-bottom: -1.5rem
}
</style>