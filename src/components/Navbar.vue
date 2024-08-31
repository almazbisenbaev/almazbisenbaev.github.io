<template>
  <header id="navbar" class="navbar">
    <div class="container container-padding">
        <nav class="nav-menu">
          <router-link to="/">About</router-link>
          <a href="//read.cv/almazb" target="_blank" rel="noopener noreferrer">CV</a>
          <a href="//medium.com/@almazbisenbaev">Blog</a>
          <router-link to="/contact">Work with me</router-link>
        </nav>
      </div>
  </header>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Navbar",
});
</script>

<style scoped>

.navbar {
  padding-top: 40px;
  padding-bottom: 40px;
}

.nav-menu {
  display: flex;
  gap: 12px;
}

.nav-menu a {
  font-family: 'General Sans', sans-serif;
  font-weight: 600;
  font-size: 13px;
  letter-spacing: 0.1em;
  line-height: 1.1;
  color: #FFFFFF;
  text-transform: uppercase;

  display: flex;
  flex-direction: row;
  align-items: center;
  padding: 12px 20px;

  border: 1px solid rgba(255, 255, 255, 0.15);
  border-radius: 99px;

  transition: 0.2s;
}

.nav-menu a:hover, .nav-menu a:focus {
  border-color: #fff;
}

</style>
