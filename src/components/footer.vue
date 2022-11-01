<template>
    <footer>
       <figure class="logo">
            <img src="@/assets/noel.svg" alt="papai noel">
            <figcaption>Feliz natal</figcaption>
       </figure>
       <nav>
            <ul>
                <li> <a href="https://github.com/dlavinia"><img src="@/assets/github.svg" title="GitHub" alt="GitHub"></a></li>
                <li> <a href="https://www.linkedin.com/in/d%C3%A9bora-melo-8b03aa205/"><img src="@/assets/linkedin.svg" title="Linkedin" alt="=LinkedIn"></a></li>
                <li> <a href="emailto:dlavinia2003@gmail.com"><img src="@/assets/gmail.svg" title="Email" alt="Email"></a></li>
            </ul>
       </nav>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'FooterPage',
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
    footer{
        background-color: #fff;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding:3rem 5rem;
    }
    nav{
        width: 15%;
    }
    ul{
        display: flex;
        justify-content: space-between;
        list-style: none;

    }

    img{
        width: 54px;
    }
    a{
        padding: 8px;
        font-size: 22px;
        font-weight: 500;
        color: var(--dark-color-text);
    }

    @media only screen and (max-width: 600px) {
        .logo{ display: none;}
        nav{ width: 100%;}
    }
  </style>
  