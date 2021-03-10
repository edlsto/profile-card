<template>
  <div id="app">
    <Background class="background" />
    <Card class="card" />
  </div>
</template>

<script>
import Card from "./components/Card.vue";

import Background from "./components/Background.vue";
export default {
  name: "App",
  components: {
    Card,
    Background,
  },
};
</script>

<style lang="sass">
@import url("https://fonts.googleapis.com/css2?family=Kumbh+Sans:wght@400;700&display=swap")

*
  margin: 0

#app
  font-family: "Kumbh Sans", sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
  height: 100vh
  width: 100vw
  display: flex
  justify-content: center
  align-items: center

.background
  position: absolute
  height: 100vh
  width: 100vw
  background: hsl(185, 75%, 39%)
  overflow: hidden

.card
  z-index: 1
</style>
