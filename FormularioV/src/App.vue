<template>
  <div class="">
    <Header />
    <Formulario/>
    
   
    
    <hr/>

   <!-- <form @submit.prevent="addUser">
      <div>
        <label>
        Nombre:<input v-model="nombre" type="text" placeholder="Nombre" required />
      </label>
      </div>
      
      <div>
        <label>
        Edad:<input v-model="edad" type="number" min="15" max="80" placeholder="edad" required />
      </label>
      </div>
      
      <div>
        <label>
        Correo Electronico<input v-model="correo" type="email" placeholder="email@email.com" required />
      </label>
      </div>
      
      
      <button type="submit">Enviar</button>
    </form>
    
    <form>
  <div class="mb-3">
    <label for="exampleInputEmail1" class="form-label">Email address</label>
    <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
    <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
  </div>
  <div class="mb-3">
    <label for="exampleInputPassword1" class="form-label">Password</label>
    <input type="password" class="form-control" id="exampleInputPassword1">
  </div>
  <div class="mb-3 form-check">
    <input type="checkbox" class="form-check-input" id="exampleCheck1">
    <label class="form-check-label" for="exampleCheck1">Check me out</label>
  </div>
  <button type="submit" class="btn btn-primary">Submit</button>
</form>
-->



  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Formulario from "./components/formulario.vue"
export default{
  components: {
    Formulario,
    Header,
  }
}
  
</script>

<style scoped>

</style>