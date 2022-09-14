<template>
  <main class="container">
    <Suspense>
      <template #default>
        <FeaturedMovie />
      </template>
      <template #fallback> Loading... </template>
    </Suspense>
  </main>
</template>

<script>
import FeaturedMovie from "@/components/FeaturedMovie.vue";
export default {
  components: {
    FeaturedMovie,
  },
};
</script>

<style lang="scss" scoped></style>
