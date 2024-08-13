<script>

export default {
  name: 'EquipeView',
  data() {
    return {
      equipe: [
        { id: 1, nome: 'João Pedro', img: '../../public/joao.jpeg', cargo: 'Back-End / Auxiliar' },
        { id: 2, nome: 'Matheus Gaspar', img: '../../public/matheusg.png', cargo: 'Back-End / Geral' },
        { id: 3, nome: 'Enrique Cardoso', img: '../../public/enrique.jpg', cargo: 'Front-End (auxiliar)' },
        { id: 4, nome: 'Nicolas Sestrem', img: '../../public/nicolas.jpg', cargo: 'Figma' },
        { id: 5, nome: 'Manoel Dias', img: '../../public/manoel.png', cargo: 'Front-End (principal)' },
        { id: 6, nome: 'Kaue Ian', img: '../../public/kaue.jpg', cargo: 'RNF, RF, RN' }
      ]
    }
  }
}

</script>

<template>
  <div class="container">
    <div v-for="membro in equipe" :key="membro.id" class="membro">
      <img :src="membro.img" alt="Imagem do membro" width="100" height="100">
      <p><span>{{ membro.nome }}</span></p>
      <p>{{ membro.cargo }}</p>
    </div>
  </div>
</template>

<style scoped>

header {
  line-height: 1.5;
  max-height: 100vh;
}
.container {
  display: flex;
  flex-wrap: wrap;
  margin-top: 20vh;
  margin-bottom: 20vh;
  background-color: rgb(158, 157, 157);
  padding: 20px;
  text-align: center;
}

.membro {
  flex: 1 1 calc(33.333% - 20px);
  margin: 10px;
  box-sizing: border-box;
}

.membro img {
  border-radius: 48%;
  border: 2px solid black;
  margin-bottom: 10px;
}

span {
  font-weight: bold;
  font-size: 15pt
}

.membro p {
  font-size: 11pt;
}


</style>