<template>
  <section class="diploma">
    <DiplomaTop />
    <DiplomaMiddle />
    <DiplomaBottom />
  </section>
</template>

<script>
import DiplomaTop from "./Diploma-top";
import DiplomaMiddle from "./Diploma-middle";
import DiplomaBottom from "./Diploma-bottom";

export default {
  name: "diploma",
  components: {
    DiplomaTop,
    DiplomaMiddle,
    DiplomaBottom,
  },
};
</script>

<style scoped>
.diploma {
  border-radius: 20px;
  background: #fafafa;
  padding: 0 05em;
  margin: 01em 4em;
  box-shadow: 0em 0em 0.125em;
  flex: 1;
  color: #4d4b4b;
}

@media (max-width: 768px), (orientation: portrait) {
  .diploma {
    margin: 0.015em;
    padding: 1.5em;
  }
}
</style>
