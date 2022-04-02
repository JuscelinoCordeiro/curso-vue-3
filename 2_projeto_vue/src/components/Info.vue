<template>
    <div>
        <p v-if="esta_trabalhando">Estou estudando as sequintes tecnologias:</p>
        <p v-else>Estou a procura de conhecimento.</p>
        <ul>
            <li>PHP</li>
            <li>Laravel</li>
            <li>InertiaJs</li>
            <li>Vue</li>
        </ul>
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
            mostrar_email: true,
            email: 'suporte@vue.com.br',
            meu_link: 'https://www.google.com',
        };
    },
};
</script>
