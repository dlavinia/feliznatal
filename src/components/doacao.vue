<template>
    <section class="container">
      
        <figure>
            <img src="@/assets/shared.png" alt="">
        </figure>
        <section class="infos">
            <h1>Comemore com <br> muito amor!</h1>
            <p>Nestes feriados, festeje com muito amor e paz,<br>oferecendo muitas bênçãos aos nossos entes queridos,<br>amigos e vizinhos, desejando-lhes um Feliz Natal.</p>
            <BotaoDoar></BotaoDoar>
        </section>
    </section>
</template>
<script>
import BotaoDoar from '@/components/botaodoar.vue';
  export default {
    name: "DoacaoSection",
    components: { BotaoDoar }
}</script>
<style scoped>
    .container{
        background-color: var(--main-color);
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 3rem 0;
        
    }
    .infos{
        flex-direction: column;
        width: 46%;
    }
   
    figure{
        width: 50%;
        display: flex;
        justify-content: center;
    }
    img{
        width: 65%;
    }
</style>