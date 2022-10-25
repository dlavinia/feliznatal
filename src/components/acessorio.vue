<template>
    <section>
        <img v-bind:src=img />
        <h2>{{titulo}}</h2>
        <p>{{texto}}</p>
    </section>
</template>
<script>
export default {
    name: 'AcessorioItem',
    props: {
        titulo: String,
        texto: String,
        img: String
    }
}

</script>
<style scoped>
section {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    width: 350px;
    padding: 20px;
}
h2{
    color: var(--dark-color-text);
    font-weight: 500;
}
p{
    text-align: center;
}

</style>