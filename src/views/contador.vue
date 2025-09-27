<template>
  <section class="section contador-section">
    <div class="container has-text-centered">
      <h1 class="title has-text-white">Página de contador</h1>

      
      <HelloWorld 
        :count="contador" 
        msg="Contador de 2 en 2" 
        @increment="incrementar" 
        @decrement="decrementar" 
      />
    </div>
  </section>
</template>

<script>
import HelloWorld from '../components/HelloWorld.vue'

export default {
  name: 'Contador',
  components: {
    HelloWorld
  },
  data() {
    return {
      contador: 0
    }
  },
  methods: {
    incrementar(n = 2) {
      this.contador += n
    },
    decrementar(n = 2) {
      this.contador -= n
      if (this.contador < 0) {
        this.contador = 0
      }
    }
  }
}
</script>

<style scoped>
.contador-section {
  min-height: 60vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #c20f0f;
}
.has-text-white {
  color: #fff;
}
</style>
