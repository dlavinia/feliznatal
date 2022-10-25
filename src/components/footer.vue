<template>
    <footer>
       <figure class="logo">
            <img src="@/assets/noel.svg" alt="papai noel">
            <figcaption>Feliz natal</figcaption>
       </figure>
       <nav>
            <ul>
                <li> <a href="#"><img src="@/assets/github.svg" title="GitHub" alt="GitHub"></a></li>
                <li> <a href="#"><img src="@/assets/linkedin.svg" title="Linkedin" alt="=LinkedIn"></a></li>
                <li> <a href="#"><img src="@/assets/gmail.svg" title="Gmail" alt="Gmail"></a></li>
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

    
  </style>
  