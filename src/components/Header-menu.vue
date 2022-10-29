<template>
    <header>
       <figure class="logo">
            <img src="@/assets/noel.svg" alt="papai noel">
            <figcaption>Feliz natal</figcaption>
       </figure>
       <nav>
            <ul>
                <li> <a href="#inicio">Início</a></li>
                <li> <a href="#acessorios">Início</a></li>
                <li> <a href="#doacao">Doação</a></li>
                <li> <a href="#contato">Contato</a></li>
            </ul>
       </nav>
    </header>
  </template>
  
  <script>
  export default {
    name: 'HeaderMenu',
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
        width: 33%;
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

    
  </style>
  