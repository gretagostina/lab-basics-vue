<template>
    <div v-for="(post, index) in posts" :key="index">
      <ul>
        <li>
          <h3>{{ index }} - {{ post.title }}</h3>
          <h5>{{ post.description }}</h5>
          <p>{{ post.content }}</p>
        </li>
      </ul>
    </div>
  </template>
  
  <script setup>
  import { ref } from "vue";
  const posts = ref([
    {
      title: "lorem",
      description:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      content: "Lorem ipsum dolor sit amet",
    },
    {
      title:
        "ipsum",
      description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      content: "consectetur adipiscing elit",
    },
    {
      title: "dolor",
      description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      content: "sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
    },
  ]);
  </script>
  
  <style>
  li {
    margin: 2rem 0;
    list-style: none;
  }
  </style>