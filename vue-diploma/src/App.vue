<template>
  <div id="app" class="parent">
    <header class="header section">Header</header>
    <main class="main section">
      <diploma> </diploma>
    </main>
    <footer class="footer section">Footer Content</footer>
  </div>
</template>

<script>
import diploma from "./components/Diploma";

export default {
  name: "App",
  components: {
    diploma,
  },
};
</script>

<style>
body {
  margin: 0em;
  display: flex;
  flex-direction: column;
  font-size: 0.9rem;
}

#app {
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

.parent {
  flex: 1;
  flex-direction: column;
}

.footer,
.header {
  background-color: #1e1c1c;
  color: white;
}
.main {
  background-color: #c4cacd;
  display: flex;
  justify-content: center;
}

.section {
  padding: 1em;
}

@media (max-width: 768px), (orientation: portrait) {
  body {
    font-size: 1.5rem;
  }
}
</style>
