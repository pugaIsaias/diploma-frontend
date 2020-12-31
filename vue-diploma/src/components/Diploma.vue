<template>
  <section class="diploma">
    <Title />
    <img alt="hyrule crest" src="../assets/crest.png" />

    <img
      alt="organization logo: hyrule"
      src="../assets/organization-logo.png"
    />
  </section>
</template>

<script>
import Title from "./Title.vue";

export default {
  name: "diploma",
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

.diploma {
  border-radius: 20px;
  background: #fafafa;
  padding: 0 05em;
  margin: 01em 4em;
  box-shadow: 0em 0em 0.125em;
  flex: 1;
  color: #4d4b4b;
}
</style>
