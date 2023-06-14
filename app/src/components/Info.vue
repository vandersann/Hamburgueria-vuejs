<template>
<div>
    <p v-if="esta_trabalhando">Estou trabalhando no momento! </p>
    <p v-else>Estou em busca de novas oportunidades</p>
    <p> Atualmente utilizando as seguintes tecnologias:</p>
    <ul>
        <li>Vue.JS</li>
        <li>JavaScript</li>
        <li>Ionic</li>
    </ul>
    <p v-show="mostrar_email"> Entre em contato via: {{ email }}</p>
</div>
</template>
<script>
    export default{
        name: 'Info',
        data() {
            return {
                esta_trabalhando: true,
                mostrar_email: true,
                email:"vandersann@gmail.com"
            }
        }
    }
</script>