<template>
  <HelloWorld msg="Welcome to Your Vue.js App" />
  <FormTest></FormTest>
  <VueFormHook></VueFormHook>
</template>

<script setup>
import HelloWorld from "./components/HelloWorld.vue";
import FormTest from "@/components/FormTest.vue";
import VueFormHook from "@/components/VeeValidation.vue";
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
