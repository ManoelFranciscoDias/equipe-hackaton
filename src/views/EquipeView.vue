<script>
export default {
    name: 'EquipeView',
    data() {
        return {
            equipe: [
                {
                    nome: 'João Pedro Dums (Santos)',
                    cargo: 'Back-End'
                },
                {
                    nome: 'Matheus Gaspar (Pito)',
                    cargo: 'Back-End / Geral'
                },
                {
                    nome: 'Enrique Cardoso (Doso)',
                    cargo: 'Front-End (auxiliar)'
                },
                {
                    nome: 'Nicolas Sestrem (Kito)',
                    cargo: 'Figma'
                },
                {
                    nome: 'Manoel Dias (Nel)',
                    cargo: 'Front-End (principal)'
                },
                {
                    nome: 'Kaue (Doka)',
                    cargo: 'RNF, RF, RN'
                }
            ]
        }
    }
}
</script>

<template>
    <div>
        <h1>Equipe</h1>
        <ul>
            <li v-for="membro in equipe" :key="membro.nome">
                <h2>{{ membro.nome }}</h2>
                <p>{{ membro.cargo }}</p>
            </li>
        </ul>
    </div>
</template>

<style scoped>
/* Your component-specific styles go here */
</style>