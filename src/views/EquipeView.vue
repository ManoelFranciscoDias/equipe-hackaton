<script>

export default {
    name: 'EquipeView',
    data() {
        return {
            equipe: [
                {
                    img: '../components/imgs/santos.png',
                    nome: 'João Pedro Dums',
                    cargo: 'Back-End'
                },
                {
                    img: '../components/imgs/matheus.png',
                    nome: 'Matheus Gaspar',
                    cargo: 'Back-End / Geral'
                },
                {
                    img: '../components/imgs/enrique.png',
                    nome: 'Enrique Cardoso',
                    cargo: 'Front-End (auxiliar)'
                },
                {
                    img: "../components/imgs/nicolas.png",
                    nome: 'Nicolas Sestrem',
                    cargo: 'Figma',
                },
                {
                    img: '../components/imgs/manoel.png',
                    nome: 'Manoel Dias',
                    cargo: 'Front-End (principal)'
                },
                {
                    img: '../components/imgs/kaue.png',
                    nome: 'Kaue Ian',
                    cargo: 'RNF, RF, RN'
                }
            ]
        }
    }
}

</script>

<template>
    <div class="container">
        
        <ul >
            <h1 class="titulo">Equipe</h1>
            <li v-for="membro in equipe" :key="membro.nome">
                
                <img v-if="membro.img" :src="membro.img" alt="Imagem do membro" width="100" height="100">
                <img v-else src='../components/imgs/sem-foto.png' alt="Imagem do membro" width="100" height="100">
                <h2>{{ membro.nome }}</h2>
                <p>{{ membro.cargo }}</p>
            </li>
        </ul>
    </div>
</template>

<style scoped>
body {
    background-color: blue;
}


.container {
    
    display: flex;
    justify-content: center;
    margin-top: 100px;
}

.titulo {
    color: black;
    font-size: 50px;
    text-align: center;
    margin-bottom: 50px;
}

</style>