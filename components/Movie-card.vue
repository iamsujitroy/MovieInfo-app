<template>
  <div class="movie-card">
    <img class="movie-thumbnail" :src="imgUrl" :alt="imgAlt" />
    <h2 class="movie-name">{{ name }}</h2>
    <span class="release-date">{{ releaseDate }}</span>
  </div>
</template>

<style>
@import "@/assets/design/custom/components/movie-card.css";
</style>

<script>
export default {
  props: ["name", "imgUrl", "imgAlt", "releaseDate"],
};
</script>
