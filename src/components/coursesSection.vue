<template>
  <div class="row ps-5">
    <courseCard v-for="i in 9" :key="i"></courseCard>
  </div>
</template>

<script>
import courseCard from "./courseCard.vue";

export default {
  components: {
    courseCard,
  },
};
</script>

<style>
</style>