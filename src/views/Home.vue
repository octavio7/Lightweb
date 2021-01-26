<template>
  <div class="home">
         <Particles
     class="particlescss"
      id="tsparticles"
      :options="{
            background: {
                color: {
                    value: 'white'
                }
            },
            fpsLimit: 60,
            interactivity: {
                detectsOn: 'canvas',
                events: {
                    onClick: {
                        enable: true,
                        mode: 'push'
                    },
                    onHover: {
                        enable: false,
                        mode: 'repulse'
                    },
                    resize: true
                },
                modes: {
                    bubble: {
                        distance: 400,
                        duration: 2,
                        opacity: 0.8,
                        size: 40
                    },
                    push: {
                        quantity: 4
                    },
                    repulse: {
                        distance: 200,
                        duration: 0.4
                    }
                }
            },
            particles: {
                color: {
                    value: '#e6e600'
                },
                links: {
                    color: '#e6e600',
                    distance: 150,
                    enable: true,
                    opacity: 0.5,
                    width: 1
                },
                collisions: {
                    enable: true
                },
                move: {
                    direction: 'right',
                    enable: true,
                    outMode: 'out',
                    random: false,
                    speed: 4,
                    straight: false
                },
                number: {
                    density: {
                        enable: true,
                        value_area: 800
                    },
                    value: 30
                },
                opacity: {
                    value: 0.5
                },
                shape: {
                    type: 'circle'
                },
                size: {
                    random: true,
                    value: 5
                }
            },
            detectRetina: true
        }"
    />
     <main class="container content d-flex">
    <div class="align-self-center">
      <h1 class="inner_txt">Páginas y aplicaciones web increíbles a tu alcance!</h1>
      <p>Descubre cómo una pagina web profesional, impulsa tu negocio Online. No basta con tener presencia en internet
        para competir, necesitas estar a la última en tecnologías web para cumplir tus metas.
        Todo lo que necesitas...</p>
         <Boton />
    </div>

  </main>
       

  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Particles from '@/components/Particles.vue'; // @ is an alias to /src
import Boton from '@/components/Boton.vue'; // @ is an alias to /src


@Component({
  components: {
    Particles,
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
 main{
   min-height:80vh;
}
 .particlescss{
  position: absolute;
  width: 100%;
  height: 90vh;
  z-index: -1;
}
.btn{
  color:red;
  z-index: 2;
}
</style>