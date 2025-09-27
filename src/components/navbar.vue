<template>
  <nav class="navbar">
    <div class="navbar-brand">
      <router-link class="navbar-item" to="/">
        <img src="https://upload.wikimedia.org/wikipedia/commons/9/95/Vue.js_Logo_2.svg" alt="Vue Logo" style="height:40px;">
      </router-link>
      <a
        role="button"
        class="navbar-burger"
        :class="{ 'is-active': isActive }"
        @click="toggleNavbar"
        aria-label="menu"
        :aria-expanded="isActive.toString()"
      >
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>

    <div class="navbar-menu" :class="{ 'is-active': isActive }">
      <div class="navbar-start">
        <router-link class="navbar-item" to="/">Home</router-link>
        <router-link class="navbar-item" to="/about">About</router-link>
        <router-link class="navbar-item" to="/services">Services</router-link>
        <router-link class="navbar-item" to="/contact">Contact</router-link>
        <ul style="list-style: none; margin: 0; padding: 0; display: flex;">
          <li style="margin-right: 10px;">
            <a href="https://www.google.com" target="_blank">Google</a>
          </li>
          <li style="margin-right: 10px;">
            <a href="https://www.github.com" target="_blank">GitHub</a>
          </li>
          <li>
            <a href="https://www.microsoft.com" target="_blank">Microsoft</a>
          </li>
        </ul>
      </div>
      <div class="navbar-end">
        <div class="navbar-item">
          <div class="buttons">
            <router-link class="button is-primary" to="/signup">
              <strong>Sign up</strong>
            </router-link>
            <router-link class="button is-light" to="/login">
              Log in
            </router-link>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isActive: false
    }
  },
  methods: {
    toggleNavbar() {
      this.isActive = !this.isActive;
    }
  }
}
</script>