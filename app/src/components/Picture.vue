<template>
    <img :src="avatar" :alt="descricao">
</template>
<script>
export default {
    name: 'Picture',
    data() {
        return {
            avatar:"/img/avatar.png",
            descricao:"Vander Sandino"
        }
    }
}
</script>