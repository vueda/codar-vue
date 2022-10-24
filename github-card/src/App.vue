<template>
  <github-card v-for="user in users" :key="user" :username="user" />
</template>

<script setup>
import GithubCard from "./components/GithubCard.vue";
const users = ["vueda"];
</script>
