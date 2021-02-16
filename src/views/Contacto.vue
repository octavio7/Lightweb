<template>
  <div class="container align-items-center col-md-4">
    <h1>Contactanos!</h1>
    <form>
      <div class="mb-3">
        <label for="nombre" class="form-label">Nombre</label>
        <input
          class="form-control"
          id="nombre"
          type="text"
          placeholder="Ronaldo Trump"
          aria-label="default input example"
        />
      </div>
      <div class="mb-3">
        <label for="InputEmail1" class="form-label">Email</label>
        <input
          type="email"
          class="form-control"
          id="InputEmail1"
          aria-describedby="emailHelp"
          placeholder="mymail@example.com"
        />
        </div>
       <div class="mb-3">
        <label for="number" class="form-label">Número</label>
        <input
          class="form-control"
          id="number"
          type="text"
          placeholder="+56 9 12345678"
          aria-label="default input example"
        />
        <div id="emailHelp" class="form-text">
          Tu información no sera compartida con nadie.
        </div>
      </div>
      
      
      <div class="mb-3">
        <label for="Textarea1" class="form-label"
          >Comentanos que buscas y nos pondremos en contacto a la brevedad!</label
        >
        <textarea
          class="form-control"
          id="Textarea1"

          rows="3"
        ></textarea>
      </div>
      <div class="col-12">
    <button class="btn btn-primary" type="submit">Enviar</button>
  </div>
    </form>
  </div>
</template>
<style scoped>
.blue {
  color: royalblue;
}

</style>
