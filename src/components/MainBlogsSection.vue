<template>
  <!-- <div class="w-full flex flex-row bg-red-300 font-bold">SDDDDDDDDDDDDDDD</div> -->
  <div class="tabs flex flex-row cursor-pointer border-b-2 border-gray-600">
    <a
      v-on:click="activetab = '1'"
      v-bind:class="[activetab === '1' ? 'active' : '']"
      >FOLLOWING</a
    >
    <a
      v-on:click="activetab = '2'"
      v-bind:class="[activetab === '2' ? 'active' : '']"
      >RECOMMENDED FOR YOU</a
    >
  </div>
  <div class="container h-screen">
    <div v-if="activetab === '1'" class="tabcontent">
      FOLLOWING
      <Blogs :articlesList="theArticlesList" />
    </div>
    <div v-if="activetab === '2'" class="tabcontent">
      RECOMMENDED FOR YOU
      <Blogs :articlesList="theArticlesList" />
    </div>
  </div>
</template>
<script>
import Blogs from "./Blogs";

export default {
  name: "MainBlogsSection",
  data() {
    return {
      activetab: "1",
      theArticlesList: [
        {
          author: {
            id: "1",
            name: "Sherlock Holmes",
            profileUrl: "https://i.pravatar.cc/150?img=13",
          },
          id: "1",
          title: "A Beginner’s Guide to Canvas with Some Real Funny Demos",
          description: "Create animation and make your website more beautiful.",
          publish_date: "12 Sept",
          duration: "2 min",
          category: "Programming",
          source: "From Your Network",
          bookmark: [],
          name: "42",
          blogImageUrl:
            "https://www.appdemovideos.com/wp-content/uploads/2017/02/photo_39424_20150718.jpg",
          tag: ["Life", "Question"],
        },
        {
          author: {
            id: "1",
            name: "Sherlock Holmes",
            profileUrl: "https://i.pravatar.cc/150?img=13",
          },
          id: "2",
          title: "A Beginner’s Guide to Canvas with Some Real Funny Demos",
          description: "Create animation and make your website more beautiful.",
          publish_date: "12 Sept",
          duration: "2 min",
          category: "Programming",
          source: "From Your Network",
          bookmark: [],
          name: "42",
          blogImageUrl:
            "https://www.appdemovideos.com/wp-content/uploads/2017/02/6-Pixabay-1024x682.jpg",
          tag: ["Life", "Question"],
        },
      ],
      myNetworkArticlesList: [
        {
          author: {
            id: "1",
            name: "Sherlock Holmes",
            profileUrl: "https://i.pravatar.cc/150?img=13",
          },
          id: "1",
          title: "A Beginner’s Guide to Canvas with Some Real Funny Demos",
          description: "Create animation and make your website more beautiful.",
          publish_date: "12 Sept",
          duration: "2 min",
          category: "Programming",
          source: "From Your Network",
          bookmark: [],
          name: "42",
          tag: ["Life", "Question"],
        },
        {
          name: "42",
          tag: ["Life", "Question"],
          duration: "6",
        },
        {
          name: "42",
          tag: ["Life", "Question"],
          duration: "6",
        },
      ],
      recommendedArticlesList: [
        {
          name: "41",
          tag: ["Life", "Question"],
          duration: "1",
          source: "From Your Network",
        },
        {
          name: "41",
          tag: ["Life", "Question"],
          duration: "3",
        },
        {
          name: "41",
          tag: ["Life", "Question"],
          duration: "4",
        },
      ],
    };
  },
  components: {
    Blogs,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.active {
  /* background: red; */
  font-weight: 700;
  padding-bottom: 4px;
  border-bottom: 1px solid 1px solid rgb(43, 43, 43, 1);
  letter-spacing: 0.077em;
  padding-right: 12px;
  /* text-decoration: underline; */
}
.tabs {
  border-bottom: 1px solid 1px solid rgba(41, 41, 41, 1);
}
</style>