<template>
  <div class="flex flex-row w-screen py-3">
    <!-- <div class="text-gray-800 mt-1 py-1">Blogs sccrrrr</div> -->
    <ul class="flex flex-col overflow-y-hidden overflow-y-scroll no-scrollbar">
      <li
        v-for="(article, index) in articlesList"
        v-bind:key="index"
        class="mx-2 list-none w-auto whitespace-no-wrap"
      >
        <Blog :article="article" class="" />
      </li>
    </ul>
  </div>
</template>

<script>
import Blog from "./Blog";

export default {
  name: "Blogs",
  props: {
    articlesList: Array,
    // required: true,
  },
  data() {
    return {};
  },
  components: {
    Blog,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* Hide scrollbar for Chrome, Safari and Opera */
.no-scrollbar::-webkit-scrollbar {
  display: none;
}

/* Hide scrollbar for IE, Edge and Firefox */
.no-scrollbar {
  -ms-overflow-style: none; /* IE and Edge */
  scrollbar-width: none; /* Firefox */
}
</style>
