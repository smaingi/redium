<template>
  <div id="app">
    <Headerr name="Medium" />
    <Body msg="I am the body" />
    <!-- <HelloWorld msg="Hello Vue3 + Tailwind.." /> -->
  </div>
</template>

<script>
import Headerr from "./components/Headerr";
import Body from "./components/Body";
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  data() {
    return {};
  },
  components: {
    HelloWorld,
    Headerr,
    Body,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 0px;
}
</style>
