<template>
  <div class="bg-gray-300 mt-1 h-2.5 px-5 py-1 cursor-pointer rounded-2xl">
    {{ topic }}
  </div>
</template>

<script>
export default {
  name: "ReadBlog",
  props: {
    topic: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
