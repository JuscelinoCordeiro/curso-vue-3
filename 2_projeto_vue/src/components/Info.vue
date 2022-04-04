<template>
    <div>
        <p v-if="esta_trabalhando">Estou estudando as sequintes tecnologias:</p>
        <p v-else>Estou a procura de conhecimento.</p>
        <p>Utilizao as seguintes tecnlogias para backend:</p>
        <ul>
            <li v-for="(tecnology, index) in backendTec" v-bind:key="index">{{ tecnology }}</li>
        </ul>
        <p>Utilizao as seguintes tecnlogias para frontend:</p>
        <ul>
            <li v-for="tecnology in frontntTec" :key="tecnology.id">{{ tecnology.language }}</li>
        </ul>
        <div>
            <button @click="showEmail">{{ textoBotao }}</button>
        </div>
        <p v-show="mostrar_email">Entre em contato pelo email {{ email }}</p>
        <!--        <p>Para acessar o portifólio basta clicar <a v-bind:href="meu_link" target="_blank">aqui</a></p>-->
        <p>Para acessar o portifólio basta clicar <a v-bind:href="meu_link" target="_blank">aqui</a></p>
    </div>
    <Picture />
</template>
<script>
import Picture from '@/components/Picture';

export default {
    name: 'InfoItem',
    components: {Picture},
    data() {
        return {
            esta_trabalhando: false,
            mostrar_email: false,
            email: 'suporte@vue.com.br',
            meu_link: 'https://www.google.com',
            textoBotao: 'Mostrar email',
            backendTec: ['PHP', 'laravel', 'Javascript', 'Python'],
            frontntTec: [
                {id: 1, language: 'HTML'},
                {id: 2, language: 'CSS'},
                {id: 3, language: 'Vue'},
            ],
        };
    },
    methods: {
        showEmail() {
            // console.log(this.email);
            this.mostrar_email = !this.mostrar_email;
            if (!this.mostrar_email) {
                this.textoBotao = 'Mostrar email';
            } else {
                this.textoBotao = 'Esconder email';
            }
        },
    },
};
</script>
