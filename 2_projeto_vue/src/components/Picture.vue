<template>
    <img :src="avatar" :alt="descricao" />
</template>

<script>
export default {
    name: 'PictureItem',
    data() {
        return {
            avatar: '/img/cod.jpg',
            descricao: 'Cod',
        };
    },
};
</script>
