<template>
    <div>
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

export default {
    name: 'App',
    components: {
        PrimeiroComponente,
        LifeCycle,
        PessoaItem,
    },
};
</script>
