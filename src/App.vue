<template>
  <div>
    <img src="./logo.png" />
    <h1>Hello Vue 3!</h1>
    <button @click="inc">Clicked {{ count }} times.</button>
  </div>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    const count = ref(0);
    const inc = () => {
      count.value++;
    };

    return {
      count,
      inc,
    };
  },
};
</script>

<style scoped>
img {
  width: 200px;
}
h1 {
  font-size: 200px;
  text-align: center;
  font-family: Arial, Helvetica, sans-serif;
}
</style>
