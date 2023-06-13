<template>
    <div>
        <h2>Essa é a descrição da pessoa: {{ name }}</h2>

    </div>
</template>

<script>
    export default {
        name: 'Pessoa',
        data() {
            return {
                name: 'Vander',
            }
        }
    }
</script>

<style lang="stylus" scoped>
</style>
