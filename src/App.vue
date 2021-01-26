<template>
  <div id="app">
 
   <nav class="navbar navbar-expand-lg navbar-light bg-custom">
    <div class="container-fluid text-center">
      <a class="navbar-brand title" href="#">LightWeb</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
        aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
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
            <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
    <router-view/>
     <footer class="footer mt-auto py-3">
    <div class="container">
      <span class="text-muted">{{copyright+currentDate.getFullYear()+marca}}</span>
    </div>
  </footer>
  </div>   
</template>
<script>
export default {
    data(){
     return {
        copyright: '\u00A9',
        marca: ' LightWeb',    
        currentDate: new Date,
        }
 }
}
</script>
<style>


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
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
@import url('https://fonts.googleapis.com/css2?family=Oleo+Script&family=Roboto:wght@100&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Oleo+Script&family=Press+Start+2P&family=Roboto:wght@100&display=swap');
.title{
    font-family: 'Oleo Script', cursive;
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
    flex-shrink: 0;
    background-color: #232f3ee5;
    border-top-left-radius: 15px;
    border-top-right-radius: 15px;
    z-index: 1;
    border-style: solid;
    border-width: 2px;
    border-color: goldenrod;
}
a {
    color: honeydew !important
}

</style>
