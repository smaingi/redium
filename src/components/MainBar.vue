<template>
  <div class="flex flex-col md:w-2/3 w-screen">
    <h1 class="text-6xl text-center bg-blue-200">MainBar</h1>
    <YourTopics />
    <FollowingProfileAvatars />
    <MainBlogsSection />
    <!-- <Blogs /> -->
  </div>
</template>

<script>
import YourTopics from "./YourTopics";
import FollowingProfileAvatars from "./FollowingProfileAvatars";
import MainBlogsSection from "./MainBlogsSection";

export default {
  name: "MainBar",
  props: {
    msg: String,
  },
  data() {
    return {};
  },
  components: {
    YourTopics,
    FollowingProfileAvatars,
    MainBlogsSection,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>