<template>
    <div>
        <h1>Olá Mundo!!!</h1>
        <PrimeiroComponente />
        <LifeCycle />
    </div>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';

export default {
    name: 'App',
    components: {
        PrimeiroComponente,
        LifeCycle,
    },
};
</script>
