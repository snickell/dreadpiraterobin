<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <div>Hi Sath!</div>
  <PersonHater name="Sath" />
  <PersonHater name="Rob" />
  <PersonHater name="Elon Musk" />
  <PersonHater name="Brownie" />
  <HelloWorld msg="Hello Vue 3 in CodeSandbox!" />
  <div>Hi Sath!</div>
  <PersonHater name="People with mental disabilities" />
</template>

<script>
import HelloWorldVue from "./components/HelloWorld.vue";
import PersonHater from "./components/PersonHater.vue";
export default {
  name: "App",
  components: {
    HelloWorld: HelloWorldVue,
    PersonHater: PersonHater,
  },
};
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
div {
  color: limegreen;
}
</style>
