<template>
  <div class="card">
    <img
      class="avatar"
      :src="user.avatar_url"
      :alt="`Foto do usuário ${user.login}`"
    />
    <h2>
      {{ user.login }}
      <span class="text-muted">{{ user.name }}</span>
    </h2>
    <p>{{ user.bio }}</p>
    <p class="text-muted">{{ user.location }}</p>
    <p class="text-muted">{{ user.company }}</p>
  </div>
</template>

<script setup>
import { ref } from "vue";

const props = defineProps({
  username: String,
});

let user = ref({});
fetch(`https://api.github.com/users/${props.username}`)
  .then((response) => response.json())
  .then((body) => (user.value = body));
</script>

<style scoped>
.card {
  background-color: #161b22;
  border-radius: 10px;
  color: white;
  font-family: Arial, Helvetica, sans-serif;
  max-width: 400px;
  padding: 20px;
  margin: 5px;
}

.avatar {
  border-radius: 50%;
  width: 100px;
}

.text-muted {
  color: #8b949e;
}
</style>
