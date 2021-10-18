<template>
  <div class="w-full h-16 bg-gray-200 shadow">
    <div
      class="cursor-pointer text-3xl px-16 py-2 text-left font-bold bg-white"
    >
      {{ appName }}
    </div>
    <!-- <hr /> -->
  </div>
</template>

<script>
export default {
  name: "Headerr",
  props: {
    name: String,
  },
  data() {
    return {
      appName: "Redium",
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
