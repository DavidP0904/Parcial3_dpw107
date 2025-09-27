<template>
  <div id="app" class="centered-app">
    <Home />
    <Contador />
    <Navbar />
    <router-view/>
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/navbar.vue'
import Footer from './components/footer.vue'
import Home from './views/home.vue'
import Contador from './views/contador.vue'

export default {
  components: {
    Home,
    Navbar,
    Contador,
    Footer
  }
}
</script>

<style>
.centered-app {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;    /* Centra horizontalmente */
  justify-content: center; /* Centra verticalmente */
  background: #c20f0f;    /* Opcional: color de fondo */
}
</style>