<template>
  <div class="flex flex-row h-16 py-3">
    <div class="text-gray-800 mt-1 py-1">YOURTOPICS</div>
    <ul class="flex flex-row overflow-x-hidden overflow-x-scroll no-scrollbar">
      <li
        v-for="(topic, index) in topicList"
        v-bind:key="index"
        class="mx-2 list-none w-auto whitespace-no-wrap"
      >
        <Topic :topic="topic" class="" />
      </li>
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
