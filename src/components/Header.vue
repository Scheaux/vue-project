<script setup>
defineProps({
  msg: String,
});
</script>

<template>
  <header>
    <h1>{{ msg }}</h1>
  </header>
</template>

<style scoped>
header {
  margin: 0;
  padding: 0;
  top: 0;
  color: #fff;
}
</style>
