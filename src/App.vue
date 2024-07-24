<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/equipe">Equipes</RouterLink>
      </nav>



  <RouterView />
</template>

<style scoped>

nav {
  background-color: white;
  height: 50px;

}


</style>
