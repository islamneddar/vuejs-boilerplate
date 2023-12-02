<template>
  <h1>Hello World!</h1>
  <p :class="titleClass">{{ msg }}</p>
  <button @click="increment">{{ count }}</button>

  <input v-model="text" placeholder="Type here" />
  <p>{{ text }}</p>

  <button @click="toggle">toggle</button>
  <h1 v-if="awesome">Vue is awesome!</h1>
  <h1 v-else>Oh no 😢</h1>
</template>

<script setup>
import { ref } from "vue";
const msg = ref("Welcome to Your Vue.js App");
const titleClass = ref("title");
const count = ref(0);
const text = ref("");
const awesome = ref(true);

function increment() {
  count.value++;
}

function toggle() {
  awesome.value = !awesome.value;
}
</script>

<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.title {
  color: red;
}
</style>
