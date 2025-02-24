<template>
  <Navigtion></Navigtion>
  <Posts v-bind:posts></Posts>
</template>

<script>
import Navigtion from "./components/Navigtion.vue";
import Posts from "./components/Posts.vue";

export default {
  components: {
    Navigtion,
    Posts,
  },
  data() {
    return {
      posts: [
        {
          id: 1,
          title: "New Beginnings",
          content: "Starting a new journey, excited for what's next!",
          date: "2025-02-24T13:00:00.000Z",
        },
        {
          id: 2,
          title: "Tech Update",
          content: "Just upgraded my phone and I'm loving the new features!",
          date: "2025-02-24T13:00:00.000Z",
        },
        {
          id: 3,
          title: "Travel Adventures",
          content:
            "Just returned from an amazing trip to Japan, can't wait to share my stories!",
          date: "2025-02-24T13:00:00.000Z",
        },
        {
          id: 4,
          title: "Book Review",
          content:
            "Just finished reading 'The Hitchhiker's Guide to the Galaxy' and it's now one of my favorites!",
          date: "2025-02-24T13:00:00.000Z",
        },
        {
          id: 5,
          title: "Foodie Fun",
          content:
            "Tried a new restaurant over the weekend and the food was incredible!",
          date: "2025-02-24T13:00:00.000Z",
        },
      ],
    };
  },
};
</script>

<style>
* {
  margin: 0;
}

body {
  background: linear-gradient(
    to bottom,
    rgb(181, 205, 221) 0%,
    rgb(90, 19, 204) 90%
  );
  height: 100vh;
}
</style>
