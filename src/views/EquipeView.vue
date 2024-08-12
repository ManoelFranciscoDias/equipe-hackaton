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
        <div v-for="membro in equipe" :key="membro.id">
            <img :src="membro.img" alt="Imagem do membro" width="100" height="100">
            <p>{{ membro.nome }}</p>
            <p>{{ membro.cargo }}</p>
        </div>
    </div>
</template>

<style scoped>


.container {

    display: flex;
    flex-wrap: wrap;
    justify-content:space-evenly;
    margin-top: 100px;
}

.titulo {
    color: black;
    font-size: 50px;
    text-align: center;
    margin-bottom: 50px;
}
</style>