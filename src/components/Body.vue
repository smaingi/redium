<template>
  <div class="w-full flex flex-row bg-blue-300">
    <MainBar />
    <SideBar />
    <!-- <main-bar></main-bar>
    <side-bar></side-bar> -->
    <!-- <div class="w-full">Shaaka Body</div> -->
  </div>
</template>

<script>
import SideBar from "./SideBar";
import MainBar from "./MainBar";

export default {
  name: "Body",
  props: {
    msg: String,
  },
  data() {
    return {};
  },
  components: {
    MainBar,
    SideBar,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
