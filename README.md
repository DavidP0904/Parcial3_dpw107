> [!NOTE]
Parcial N3
Estudiante: David Enrique Pérez Bejarano
Imagenes y caps se encuentran en la carpeta img 
Se hizo uso de vue con enlaces simples sobre redes sociales teniendo en cuenta el uso del copilot con conocimiento sobre los codigos

> [!CAUTION]
Es necesario el copiado mediante git bash en condición de windows abajo del 11 o uso simple de la terminal para activar este archivo para su mejor comprensión

> [!IMPORTANT]
Se hizo uso de vue con enlaces simples sobre redes sociales teniendo en cuenta el uso del copilot con conocimiento sobre los codigos tomando en cuenta que es un entorno virtual

> [!TIP]
Se dejo el codigo para un copiado más simple tomando en cuenta que puede usarse de forma más simple así.

```html
<template>
  <div class="hello-world">
    <h2>{{ msg }}</h2>
    <p>Valor : {{ count }}</p>
    <button class="button is-light" @click="onDecrement">Decrementar</button>
    <button class="button is-light" @click="onIncrement">Incrementar</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: {
      type: String,
      default: ''
    },
    count: {
      type: Number,
      default: 0
    }
  },
  emits: ['increment', 'decrement'],
  methods: {
    onIncrement() {
      this.$emit('increment', 2)
    },
    onDecrement() {
      this.$emit('decrement', 2)
    }
  }
}
</script>

<style scoped>
.hello-world {
  margin-bottom: 1em;
}
.button {
  margin: 0 0.5em;
}
</style>
```
