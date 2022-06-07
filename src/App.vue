<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import Header from './components/Header.vue';
import Form from './components/Form.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <Header msg="Let's Talk" />
  <Form />
  <Footer msg="OR CALL US" number="+1 555 505 5050" />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

html {
  height: 100vh;
}

body {
  background-image: url('./assets/mountains.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  background-color: #000;
}
</style>
