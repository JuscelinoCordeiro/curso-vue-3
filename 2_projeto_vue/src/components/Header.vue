<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Contato</a></li>
    </ul>
</template>

<script>
export default {
    name: 'HeaderApp',
};
</script>

<!--estylo definido somente para este componenet-->
<style scoped>
ul {
    list-style: none;
    display: flex;
    background-color: #555;
}

li {
    margin-right: 10px;
}
a {
    color: #ddd;
    text-decoration: none;
    transition: 0.5s;
}
a:hover {
    color: turquoise;
}
</style>
