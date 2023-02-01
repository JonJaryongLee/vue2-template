<template>
  <div>
    <h1>home</h1>
    <ul>
      <li>밥먹기</li>
      <li>영화보기</li>
      <li>차마시기</li>
      <button type="button" class="btn btn-primary" v-on:click="test">
        Primary
      </button>
      <span class="material-symbols-outlined"> expand_more </span>
    </ul>
  </div>
</template>

<script>
import axios from "axios";
export default {
  methods: {
    async test() {
      try {
        const response = await axios.get(
          "https://jsonplaceholder.typicode.com/todos/1"
        );
        if (response.data) {
          console.log(response.data);
        }
      } catch (error) {
        console.log(error);
      }
    },
  },
};
</script>
