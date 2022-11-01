<template>
    <header>
       <figure class="logo">
            <img src="@/assets/noel.svg" alt="papai noel">
            <figcaption>Feliz natal</figcaption>
       </figure>

       <img id="menu-mobile" v-on:click="openMenu" src="@/assets/menu-hamburguer.svg" alt="menu">
       <div id="menu-overlay"  v-on:click="closeMenu" v-if="menuActive"></div>
       <nav :class="{open:menuActive}">
            <ul>
                <li> <a href="#inicio">Início</a></li>
                <li> <a href="#acessorios">Acessórios</a></li>
                <li> <a href="#doacao">Doação</a></li>
                <li> <a href="#contato">Contato</a></li>
            </ul>
       </nav>
       
    </header>
  </template>
  
  <script>
  export default {
    name: 'HeaderMenu',
    data(){
        return{
            menuActive : false
        }
    },

    methods:{
        openMenu: function(){
            this.menuActive = true;
        },
        closeMenu: function(){
            this.menuActive = false;
        }
    }

  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
    header{
        background-color: var(--main-color);
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding:3rem 5rem;
    }
    nav{
        width: 25%;
    }
    ul{
        display: flex;
        justify-content: space-between;
        list-style: none;

    }
    a{
        padding: 8px;
        font-size: 22px;
        font-weight: 500;
        color: var(--dark-color-text);
    }
    #menu-mobile{
        display: none;
    }

    #menu-overlay{
        position: fixed;
        left: 0;
        top: 0;
        height: 100vh;
        width: 40%;
        background-color: var(--main-color);
        opacity: .6;
    }
    @media only screen and (max-width: 600px) {
        #menu-mobile{
        display: block;
        width: 30px;

    }
    header{
        padding: 1rem;
    }

    .logo img{
        width: 50px;
    }
    nav{
        position: fixed;
        top: 0;
        right: 0;
        width: 55%;
        height: 100vh;
        background-color:#fff;
        padding: 8rem 0 0 2rem;
        display: none;
        
        
    }
    .open{
        display: block;
    }
    ul{
        flex-direction: column;
    }
    li{
        margin-top: 40px;
    }
    }

  </style>
  