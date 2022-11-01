<template>
    <button>
        <img src="@/assets/gift.svg" alt="presente">
        <a href="#" target="_blank">
            Fazer uma doação
        </a>
    </button>
</template>
<script>
    export default{
        name: 'BotaoDoar'
    }
</script>
<style scoped>
    button{
        padding: 12px 32px;
        border-radius: 8px;
        border: none;
        box-shadow: none;
        background-color: var(--btn-color);
        display: flex;
        align-items: center;
        justify-content: center;
    }
    a{
        color: #fff;
        font-size: 22px;
        font-weight: 600;
        margin-left: 1rem;
    }
    img{
        width: 30px;

    }

    button:hover{
        cursor: pointer;
    }

</style>