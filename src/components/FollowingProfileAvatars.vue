<template>
  <div class="flex flex-row bg-orange-400 py-2">
    <!-- <div class="text-gray-900 mt-1 py-1 h-16">My Avatars</div> -->
    <ul class="flex flex-row overflow-x-hidden overflow-x-scroll no-scrollbar">
      <li
        v-for="(avatarProfile, index) in avatarProfileList"
        v-bind:key="index"
        class="mx-2 list-none whitespace-no-wrap"
      >
        <FollowingProfileAvatar :avatarProfile="avatarProfile" />
      </li>
    </ul>
  </div>
</template>
<script>
import FollowingProfileAvatar from "./FollowingProfileAvatar";
export default {
  name: "FollowingProfileAvatars",
  data() {
    return {
      avatarProfileList: [
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=26",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=1",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=2",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=3",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=4",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=5",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=6",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=7",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=8",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=9",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=10",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=11",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=12",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=13",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=14",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=15",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=16",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=17",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=18",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=19",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=20",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=21",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=22",
          blogLink: "",
          newBlogs: 1,
        },
        {
          name: "Sherlock Holmes",
          profileUrl: "https://i.pravatar.cc/150?img=23",
          blogLink: "",
          newBlogs: 1,
        },
      ],
    };
  },
  components: {
    FollowingProfileAvatar,
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