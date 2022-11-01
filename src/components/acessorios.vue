<template>
    <section class="container">
        <h1>Acessórios</h1>
        <p>Nessas festas de fim de ano mande um presente para <br> a pessoa amada e compartilhe a alegria do Natal.</p>

        <section class="cards">
            <AcessorioItem 
             :img="require('@/assets/giving1.png')" 
             titulo="Presentes" 
             texto="Eles são os melhores presentes que existem.">
            </AcessorioItem>

            <AcessorioItem 
             :img="require('@/assets/giving2.png')" 
             titulo="Enfeites" 
             texto="Dê uma decoração.">
            </AcessorioItem>

            <AcessorioItem 
             :img="require('@/assets/giving4.png')" 
             titulo="Doces" 
             texto="Aproveite os doces natalinos.">
            </AcessorioItem>

            <AcessorioItem 
             :img="require('@/assets/giving3.png')" 
             titulo="Muito amor" 
             texto="Aproveite os sentimentos que duram para sempre.">
            </AcessorioItem>
        </section>
    </section>
</template>
<script>
    import AcessorioItem from "@/components/acessorio.vue";
  export default {
    name: "AcessoriosSection",
    components:{
        AcessorioItem
    }
}</script>
<style scoped>
    .container{
        background-color: #fff;
        padding: 4rem 0;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
    p{
        text-align: center;
    }
    .cards{
        display: flex;
        
    }

@media only screen and (max-width: 600px) {
 .cards{
    flex-direction: column;
 }
}
</style>