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
