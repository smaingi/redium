<template>
  <!-- flex md:hidden w-2/5 md:w-11/12 mt-0 md:mt-4 items-center shadow-md -->
  <!-- hidden md:block -->
  <div class="flex md:flex hidden md:visible md:w-1/3 md:bg-red-700">
    <h1 class="w-screen text-6xl text-center bg-green-200">SideBar</h1>
  </div>
</template>

<script>
export default {
  name: "SideBar",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>