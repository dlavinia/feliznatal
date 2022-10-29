<template>
  <HeaderMenu></HeaderMenu>
  <InicioSection id="inicio"></InicioSection>
  <AcessoriosSection id="acessorios"></AcessoriosSection>
  <DoacaoSection id="doacao"></DoacaoSection>
  <FooterPage id="contato"></FooterPage>
</template>

<script>
import HeaderMenu from './components/Header-menu.vue'
import InicioSection from './components/inicio.vue'
import AcessoriosSection from './components/acessorios.vue'
import DoacaoSection from './components/doacao.vue'
import FooterPage from './components/footer.vue'

export default {
  name: 'App',
  components: {
    HeaderMenu,
    InicioSection,
    AcessoriosSection,
    DoacaoSection,
    FooterPage
  }
}
</script>

<style>
  @import './styles/global.css'; 

</style>
