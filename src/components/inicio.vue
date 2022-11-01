<template>
    <section class="container">
        <section class="infos">
            <h1>Feliz Natal e <br> Feliz Ano Novo!</h1>
            <p>Nessas festas de fim de ano mande um presente para <br>a pessoa amada e compartilhe a alegria do Natal.</p>
            <BotaoDoar></BotaoDoar>
        </section>
        <figure>
            <img src="@/assets/send.png" alt="">
        </figure>
    </section>
</template>
<script>
import BotaoDoar from '@/components/botaodoar.vue';
  export default {
    name: "InicioSection",
    components: { BotaoDoar }
}</script>
<style scoped>
    .container{
        background-color: var(--main-color);
        display: flex;
        justify-content: center;
        align-items: center;
        padding-bottom: 12%;
        height: 600px;
    }
    .infos{
        flex-direction: column;
        width: 40%;
    }
   
    figure{
        width: 45%;
    }
    img{
        width: 100%;
    }
@media only screen and (max-width: 600px) {
    .container{
        padding: 2rem;
        height: 60vh;
    }
    .infos{
        width: 100%;
        display: flex;
        justify-content: center;
        text-align: center;
        
    }
    figure{
        display: none;
    }
    }  
</style>