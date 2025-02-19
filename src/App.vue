<template>
    <Navigtion></Navigtion>
    <div v-for="post in posts" :key="post.id">
        <p>{{ post.content }}</p>
    </div>
 </template>
 
 <script>
 import Navigtion from './components/Navigtion.vue';
 
 export default {
     components: {
         Navigtion
     },
     data() {
         return {
             posts: [
                 { id: 1, content: "This is the first post" },
                 { id: 2, content: "This is the second post" }
             ]
         }
     }
 }
 </script>
 
 <style>
     * {
         margin: 0;
     }
 </style>