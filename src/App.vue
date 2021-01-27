<template>
  <div id="app" class="d-flex flex-column">
    <Particles
      class="particlescss"
      id="tsparticles"
      :options="{
        background: {
          color: {
            value: 'white',
          },
        },
        fpsLimit: 60,
        interactivity: {
          detectsOn: 'canvas',
          events: {
            onClick: {
              enable: true,
              mode: 'push',
            },
            onHover: {
              enable: false,
              mode: 'repulse',
            },
            resize: true,
          },
          modes: {
            bubble: {
              distance: 400,
              duration: 2,
              opacity: 0.8,
              size: 40,
            },
            push: {
              quantity: 4,
            },
            repulse: {
              distance: 200,
              duration: 0.4,
            },
          },
        },
        particles: {
          color: {
            value: '#e6e600',
          },
          links: {
            color: '#e6e600',
            distance: 150,
            enable: true,
            opacity: 0.5,
            width: 2,
          },
          collisions: {
            enable: true,
          },
          move: {
            direction: 'right',
            enable: true,
            outMode: 'out',
            random: false,
            speed: 3,
            straight: false,
          },
          number: {
            density: {
              enable: true,
              value_area: 800,
            },
            value: 30,
          },
          opacity: {
            value: 0.5,
          },
          shape: {
            type: 'circle',
          },
          size: {
            random: true,
            value: 6,
          },
        },
        detectRetina: true,
      }"
    />
    <nav class="navbar navbar-expand-lg navbar-light bg-custom">
      <div class="container-fluid text-center">
        <a class="navbar-brand title" href="#">LightWeb</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon navbar-text"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Features</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Pricing</a>
            </li>
            <li class="nav-item">
              <a
                class="nav-link disabled"
                href="#"
                tabindex="-1"
                aria-disabled="true"
                >Disabled</a
              >
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <div class="d-flex align-items-center altura">
    <router-view />
    </div>
    <footer class="footer mt-auto py-3 align-self-end">
      <div class="container">
        <span class="text-muted">{{
          copyright + currentDate.getFullYear() + marca
        }}</span>
      </div>
    </footer>
  </div>
</template>
<script>
import Particles from "@/components/Particles.vue"; // @ is an alias to /src
  
export default {
  components: {
    Particles,
  },
  data() {
    return {
      copyright: "\u00A9",
      marca: " LightWeb",
      currentDate: new Date(),
    };
  },
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align:left;
  color: #2c3e50;
  height: 100vh;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
@import url("https://fonts.googleapis.com/css2?family=Oleo+Script&family=Roboto:wght@100&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Oleo+Script&family=Press+Start+2P&family=Roboto:wght@100&display=swap");
.title {
  font-family: "Oleo Script", cursive;
}
.navbar {
  background-color: #232f3ee5;
  border-bottom-left-radius: 15px;
  border-bottom-right-radius: 15px;
  border-style: solid;
  border-width: 2px;
  border-color: goldenrod;
}
.footer {
  background-color: #232f3ee5;
  border-top-left-radius: 15px;
  border-top-right-radius: 15px;
  z-index: 1;
  border-style: solid;
  border-width: 2px;
  border-color: goldenrod;
  width: 100%;
}
a {
  color: honeydew !important;
}
 .particlescss{
  position: absolute;
  width: 100%;
  height: 90%;
  z-index: -1;
}
.altura{
  min-height:79%;
}
</style>
