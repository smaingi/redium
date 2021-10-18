<template>
  <div class="min-w-full w-16 my-2">
    <!-- <h1 class="text-6xl text-center bg-green-400">Following Profile Avatar</h1> -->
    <div class="relative inline-bock cursor-pointer">
      <img
        :src="avatarProfile.profileUrl"
        alt="shaaka"
        class="inline-block object-cover w-16 h-16 rounded-full"
      />
      <span
        class="absolute top-0 right-0 inline-block w-5 h-5 bg-green-600 border-2 border-white rounded-full"
      ></span>
    </div>
    <!-- {{ avatarProfile }} -->
  </div>
</template>

<script>
export default {
  name: "FollowingProfileAvatar",
  props: {
    avatarProfile: Object,
  },
  data() {
    return {};
  },
  components: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>