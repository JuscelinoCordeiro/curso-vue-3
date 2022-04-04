<template>
    <div>
        <Header />
        <h1>Olá Mundo!!!</h1>
        <PrimeiroComponente />
        <LifeCycle />
        <PessoaItem />
    </div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
import PessoaItem from './components/PessoaItem.vue';
import Header from '@/components/Header';

export default {
    name: 'App',
    components: {
        Header,
        PrimeiroComponente,
        LifeCycle,
        PessoaItem,
    },
    data() {
        return {
            testando: 'teste',
        };
    },
};
</script>
<style>
body {
    background-color: #97b8e8;
    color: #333;
}
a {
    color: red;
}
</style>
