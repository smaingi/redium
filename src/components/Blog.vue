<template>
  <!-- <div class="flex flex-row w-screen py-3">Blogged</div> -->
  <!-- <div>{{ article }}</div> -->
  <div class="flex w-full">
    <div
      class="flex-1 flex flex-col flex-wrap content w-9/12 pl-2 mb-2 bg-red-200"
    >
      <div class="author flex flex-row pt-2">
        <img
          :src="article.author.profileUrl"
          alt="shaaka"
          class="author_avatar inline-block object-cover w-5 h-5 rounded-full"
        />
        <div class="author_name ml-2 font-semibold">
          {{ article.author.name }}
        </div>
      </div>

      <div class="px-2 break-all content">
        <div class="tide max-w-full bg-red-400">
          <h2 class="title max-w-full break-all font-black">
            {{ article.title }}
          </h2>
          <div class="desc max-w-full break-all text-gray-700">
            {{ article.description }}
          </div>
        </div>
        <div class="flex flex-row meta">
          <div class="publish_date">{{ article.publish_date }}</div>
          <div class="read_duration">{{ article.duration }}</div>
          <div class="category">{{ article.category }}</div>
          <div class="source">{{ article.source }}</div>
          <div class="flex flex-row extras">
            <div class="bookmark">{{ article.bookmark }}</div>
            <div class="more">...</div>
          </div>
        </div>
      </div>
    </div>
    <!-- <div class="flex image md:w-3/12 bg-green-200 mb-2">
      <img
        :src="article.blogImageUrl"
        alt="shaaka"
        class="author_avatar inline-block object-cover rounded-sm"
        width="200"
        height="134"
      />
    </div> -->
  </div>
</template>

<script>
export default {
  name: "Blog",
  props: {
    article: Object,
    // required: true,
  },
  data() {
    return {};
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* .oow {
  overflow-wrap: break-word;
  word-wrap: break-word;
  hyphens: auto;
  flex-wrap: wrap;
} */
.content {
  /* display: block; */
  overflow-wrap: anywhere;
  max-width: 100%;

  /* margin-bottom: 48px;
  margin-left: 20px; */
}
/*  
.title {
  display: inline-block;
  text-overflow: ellipsis;
  overflow: hidden;
}
.tide {
  display: block;
} */
</style>
