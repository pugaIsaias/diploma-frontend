<template>
  <div class="res-col-to-row">
    <Title />
    <img alt="hyrule crest" src="../assets/crest.png" />
  </div>
</template>

<script>
import Title from "./Title.vue";

export default {
  name: "DiplomaTop",
  components: {
    Title,
  },
};
</script>

<style scoped>
img {
  height: 5em;
  margin: 2.5em 0;
}

.res-col-to-row {
  display: flex;
  justify-content: space-between;
}

@media (max-width: 768px), (orientation: portrait) {
  .res-col-to-row {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
}
</style>
