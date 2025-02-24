<template>
  <div class="container" v-for="post in posts" :key="post.id">
    <h2>{{ post.title}}</h2>
    <small>{{ post.date }}</small>
    <p>{{ post.content }}</p>
    <div class="btn-container">
        <button>Read More</button>
        <button>Edit</button>
        <button class="delete" v-on:click="deletePost(post.id)">Delete</button>
    </div>
  </div>
</template>

<script>
    export default {
        props: {
            posts: Array
        },
        methods: {
            deletePost(postId) {
                console.log(postId)
            }
        }
    }

  
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap");

.container {
  font-family: "Open Sans", serif;
  width: 70%;
  display: flex;
  flex-direction: column;
  margin: 0 auto;
  color: rgb(0, 0, 0);
}



.btn-container {
    margin-bottom: 20px;
}

.btn-container button {
    cursor: pointer;
}
</style>
