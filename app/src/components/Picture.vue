<template>
    <img :src="avatar" :alt="descricao">
</template>
<script>
export default {
    name: 'Picture',
    data() {
        return {
            avatar:"/app/public/img/avatar.png",
            descricao:"Vander Sandino"
        }
    }
}
</script>