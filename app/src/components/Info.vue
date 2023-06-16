<template>
<div>
    <p v-if="esta_trabalhando">Estou trabalhando no momento! </p>
    <p v-else>Estou em busca de novas oportunidades</p>
    <p> Atualmente utilizando as seguintes tecnologias para o FrontEnd:</p>
    <ul>
        <li v-for="(technology, index) in frontEnd_tech" :key="index"> {{ technology }} </li>
    </ul>
    <p> Utilizo as seguintes tecnoligas para BackEnd:</P>
    <ul>
        <li v-for="technology in backEnd_tech" :key="technology.id"> {{ technology.language }} </li>
    </ul>
    <div>
        <button @click="showEmail">{{ textoBotao }}</button>
    </div>
    <p v-show="mostrar_email"> Entre em contato via: {{ email }}</p>
    <p>Para acessar meu portfólio <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
    <Picture/>
</div>
</template>
<script>
import Picture from "./Picture.vue";

    export default{
        name: 'Info',
        components: {
            Picture
        },
        data() {
            return {
                esta_trabalhando: true,
                mostrar_email: false,
                email:"vandersann@gmail.com",
                meu_link:"https://google.com",
                textoBotao: "Mostrar Email",
                frontEnd_tech: ["JavaScript", "Vue.Js", "Ionic"],
                backEnd_tech: [
                    {id: 1, language: 'Java'},
                    {id: 2, language: 'Python'},
                    {id: 3, language: 'C++'}
                ]
            }
        },
        methods: {
            showEmail() {
                this.mostrar_email= !this.mostrar_email
                if(!this.mostrar_email) {
                    this.textoBotao= "Mostrar Email"
                } else {
                    this.textoBotao = "Esconder Email"
                }
            }
        }
    }
</script>