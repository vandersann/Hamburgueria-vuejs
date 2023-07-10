<template>
    <h2>Complete meu formulário</h2>
        <form action="" @submit="enviarForms">
            <div>
                <input type="text" v-model="name">
            </div>
            <div>
                <input type="text" v-model="email">
            </div>
            <div>
                <Submit/>
            </div>
        </form>
        <p> Teste </p>
        <p> Teste </p>
        <p> Teste </p>
</template>
<script>
    import InputText from './Form/InputText.vue';
    import Submit from './Form/Submit.vue';

    export default {
        name: 'Form',
        components: {
            InputText,
            Submit
        },
        data () {
            return {
                name: "",
                email:""
                }
        },
        methods: {
            enviarForms(e) {
                e.preventDefault(); //Ele inviabiliza eventos padrões javascript, como no caso dos formularios e o pageReload
                const name = this.name;
                const email= this.email;
                console.log("formulario enviado")
                console.log("O nome é:" + name)
            }
        }
    }
</script>

<style scoped>
    p{
        margin: 15rem;
    }
</style>