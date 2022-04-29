<template>
     
  <div>
    
    <div class="area1">
      <login-layout class="cima" Tema="Summer Dark" />
      <background-shapes class="baixo" Estilo="Summer dark" />
    </div>
    

      <!--<navHorizontal class="c2" name1="Home" name2="Sobre" name3="Contato" name4="Configurações" name5="Seus dados" /> -->

      <!--<area-comentarios Titulo="Comentários" />-->

      <!--<nav-vertical />-->
    
  </div>
 
</template>

<script>
import loginLayout from './components/loginLayout.vue'
import BackgroundShapes from './components/BackgroundShapes.vue'
//import navHorizontal from './components/navHorizontal.vue'
//import navVertical from './components/navVertical.vue'
//import areaComentarios from './components/areaComentarios.vue'

export default {
  name: 'App',
  components: {
    BackgroundShapes,
    loginLayout,
    //navHorizontal,
    //navVertical,
    //areaComentarios,
  }
}
</script>

<style>
  *{
    margin: 0;
    padding: 0;
  }

  .cima{
    position: absolute;
    z-index: 1;
  }

   .baixo{
    position: absolute;
    z-index: 0;
  }


</style>
