<template>
    <div>
        <h1>Ola vue!</h1>
        <p>Meu nome é {{ nome }}, tenho {{ idade }}, sou um {{ profissao }} .</p>
    </div>
</template>

<script>
    export default {
        name: "Primeiro",
        data() {
        return {
            nome: "Vander",
            sobrenome:"Sandino",
            idade: 32,
            profissao: "Dev. FrontEnd",
        };
    },
};
</script>
