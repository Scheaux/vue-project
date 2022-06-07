<script setup>
defineProps({
  msg: String,
  number: String,
});
</script>

<template>
  <footer>
    <div class="container">
      <hr />
      <span>{{ msg }}</span>
      <hr />
    </div>
    <h2>{{ number }}</h2>
  </footer>
</template>

<style scoped>
footer {
  margin-top: 50px;
  color: #fff;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.container {
  display: flex;
  width: 500px;
}

hr {
  width: 100%;
  height: 1px;
  border: none;
  background-color: #fff;
  opacity: 0.5;
}

span {
  white-space: nowrap;
  padding: 0 5px;
}
</style>
