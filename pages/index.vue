<template>
  <div class="container">
    <form @submit.prevent>
      <div class="input-group">
        <input v-model.lazy="query" type="text" placeholder="search weather in city">
        <input type="submit" value="search">
      </div>
    </form>

    <p>
      {{ query }}
    </p>

  </div>
</template>

<script setup>
import { ref } from 'vue';

const query = ref('')

</script>

<style  scoped>
.container {
  max-width: 1200px;
  margin: 0 auto;
}
form {
  margin: 1rem auto;
}
.input-group {
  display: flex;
  justify-content: center;
}
input[type=text] {
  width: 70%;
  padding: 0.5rem;
  font-size: 1.2rem;
  outline: none;
  border: 2px solid #6b5b95;

}
input[type=submit] {
  padding: 0.5rem;
  font-size: 1.2rem;
  border: 2px solid #6b5b95;
  border-left: none;
  background-color: #6b5b95;
  color: white;
}

</style>