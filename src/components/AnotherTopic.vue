<template>
  <div class="flex flex-row">
    <div class="bg-blue-400">YOURTOPICS</div>
    <!-- <div v-for="topic of TopicLists" :key="topic">
      <Topic :topic="topic" />
    </div> -->
    <!-- <div v-for="(topic, index) in topicList" v-bind:key="index">
      <Topic :topic="topic" />
    </div> -->
    <ul
      class="flex flex-row overflow-x-hidden overflow-x-scroll no-scrollbar h-16"
    >
      <li
        v-for="(topic, index) in topicList"
        v-bind:key="index"
        class="mx-2 list-none bg-blue-400 w-auto inline-block hover:bg-yellow-500"
      >
        <!-- {{ topic }} -->
        <Topic :topic="topic" class="bg-white" />
      </li>
      <!-- <li v-for="(topic, index) in topicList" v-bind:key="index">
      {{ topic }}
    </li> -->
    </ul>
  </div>
</template>

<script>
import Topic from "./Topic";

export default {
  name: "YourTopics",
  // props: {
  //   topicLists: Array,
  //   // required: true,
  // },
  data() {
    return {
      topicLists: ["Reddit", "Medium", "Quora", "Forest", "Dev.to"],
      topicList: [
        "Addiction",
        "Android Development",
        "Art C",
        "Artificial Intelligence",
        "Basic Income",
        "Blockchain",
        "Business",
        "Comics",
        "Cryptography",
        "Cybersecurity",
        "Data Science",
        "Disability",
        "Education",
        "Equality",
        "Family",
        "Feminism",
        "Fiction",
        "Food",
        "Freelancing",
        "Gaming",
        "Gun Control",
        "Javascript",
        "Justice",
        "Leadership",
        "Lifestyle",
        "Marketing",
        "Money",
        "Parenting",
        "Philosophy",
        "Photography",
        "Privacy",
        "Programming",
        "Psychology",
        "Race",
        "San Fransisco",
        "Science",
        "Self Driving Cars",
        "Software Engineering",
        "Space",
        "Spirituality",
        "Style",
        "Technology",
        "Transportation",
        "Travel",
        "TrueCrime",
        "UX",
        "Visual Design",
        "Work",
        "World",
      ],
    };
  },
  components: {
    Topic,
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
