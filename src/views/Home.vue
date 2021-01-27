<template>
  <div class="home container">

     <main>
    <div>
      <h1>Páginas y aplicaciones web increíbles a tu alcance!</h1>
      <p class="text-start fw-bold">Descubre cómo una página web profesional, impulsa tu negocio Online. No basta con tener presencia en internet
        para competir, necesitas estar a la última en tecnologías web para cumplir tus metas.
        Todo lo que necesitas...</p>
         <Boton />
    </div>

  </main>
       

  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Boton from '@/components/Boton.vue'; // @ is an alias to /src


@Component({
  components: {
    Boton
  },
})

export default class Home extends Vue {}

</script>
<style scoped>
 .home {
   z-index: 1;
 }
 h1 {
    color: royalblue;
    font-family: 'Press Start 2P', cursive;
    margin-bottom:1em;
}

</style>