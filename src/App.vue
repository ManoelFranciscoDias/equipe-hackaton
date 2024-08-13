<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>
    <div class="head">
      <p class="titulo">Integrantes da equipe - Hackaton</p>
    </div>
  </header>

  <RouterView />

  <footer>
    <div class="foot">
      <h1> Membros do site de locação - Hackaton</h1>
      <p>Instituto Federal Catarinense</p>
    </div>
  </footer>
</template>

<style scoped>
.titulo {
  color: white;
  font-size: 50px;
  text-align: center;
  margin-bottom: 50px;
}

.head {
  background-color: rgb(53, 32, 80);
  padding: 20px;
}

.foot {
  background-color: rgb(53, 32, 80);
  padding: 20px;

}

h1 {
  color: white;
  font-size: 20px;
}

.foot p {
  color: white;
  margin-left: 10px;
  margin-top: 10px
}
</style>
