<template>
    <div>
        <h1>Olá Vue!!!</h1>
        <p>Meu nome é {{ nome }} e eu sou {{ profissao }}</p>
    </div>
</template>

<script>
export default {
    name: 'PrimeiroComponente',
    data() {
        return {
            nome: 'juscelino',
            profissao: 'Milico',
        };
    },
};
</script>
<style>
h1 {
    color: #0d30e0;
}
</style>
