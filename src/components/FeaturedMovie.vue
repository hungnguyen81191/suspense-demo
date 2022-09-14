<template>
  <div>
    <img :src="`../../src/assets/{{movie.img}}`" alt="" />
    <div>
      <h1>{{ movie.name }}</h1>
      <p>
        {{ movie.description }}
      </p>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
const movie = ref(null);
const getMovie = async () => {
  await new Promise((resolve) => setTimeout(resolve, 3000));
  movie.value = {
    img: "logo.png",
    name: "hehehe",
    description: "hihihi",
  };
};
await getMovie();
</script>

<style lang="scss" scoped></style>
