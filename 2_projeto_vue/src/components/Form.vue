<template>
    <div>
        <h2>Meu Formulário</h2>
    </div>
    <form action="" @submit="enviarFormulario">
        <div><input type="text" v-model="name" /></div>
        <div><input type="text" v-model="email" /></div>
        <div><Submit /></div>
    </form>
    <p>Conteúdo</p>
    <p>Conteúdo</p>
    <p>Conteúdo</p>
</template>
<script>
import Submit from './form/Submit.vue';
export default {
    name: 'FormItem',
    components: {Submit},
    data() {
        return {
            name: '',
            email: '',
        };
    },
    methods: {
        enviarFormulario(e) {
            const name = this.name;
            const email = this.email;

            e.preventDefault(); //inserir para evitar o relad da pagina
            console.log('form enviado');
            console.log('name = ' + name);
            console.log('email = ' + email);
        },
    },
};
</script>
<style scoped>
p {
    margin: 50px;
}
</style>
