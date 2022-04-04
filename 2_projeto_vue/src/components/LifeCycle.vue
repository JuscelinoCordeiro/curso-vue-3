<template>
    <div>
        <h1>meu nome é: {{ nome }}</h1>
    </div>
</template>

<script>
export default {
    name: 'LifeCycle',
    data() {
        return {
            nome: 'Ainda nao sei',
        };
    },
    created() {
        setTimeout(() => {
            this.nome = 'jusce';
        }, 1000);
        this.lifeCycle();
    },
    mounted() {
        setTimeout(() => {
            this.nome = 'Elesbao';
        }, 3000);
        this.lifeCycle();
    },
    methods: {
        lifeCycle() {
            // console.log('executou ' + 'this.lifeCycle()');
        },
    },
};
</script>
