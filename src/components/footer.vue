<template>
  <footer class="footer">
    <div class="content">
      <p>
        <strong>Mi Parcial</strong> by <a href="https://github.com/DavidP0904/">David Enrique Pérez Bejarano</a>. 
      </p>
      <p>
        <a href="https://www.facebook.com/profile.php?id=100008683900339" target="_blank">Facebook</a> |
        <a href="https://twitter.com/Vidpebee" target="_blank">Twitter</a> |
        <a href="https://instagram.com/vidpebe" target="_blank">Instagram</a>
      </p>
      <p>&copy; 2025 Mi Parcial. Todos los derechos reservados.</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped>
.footer {
  background-color: #bb1f1f;
  padding: 1rem 0;
  width: 100%;
  position: relative;
  bottom: 0;
  left: 0;
}

.content {
  text-align: center;
  color: #fff;
}
</style>