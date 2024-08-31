<template>
  <div class="App">
    <navbar />
    <router-view></router-view>
    <footer-component />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Navbar from "./components/Navbar.vue";
import FooterComponent from "./components/FooterComponent.vue";

export default defineComponent({
  name: "App",
  components: {
    Navbar,
    FooterComponent,
  },
});
</script>

<style>
/* @import './assets/main.css'; */

/* .App {
  font-family: 'General Sans', 'Helvetica', 'Helvetica Neue', sans-serif;
  font-size: 1rem;
  font-weight: normal;
  color: #000;
  background: #fff;
} */
</style>
