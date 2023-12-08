<script lang="ts">
import StartScreen from "./screens/StartScreen.vue";

export default {
  name: "App",
  components: {
    StartScreen,
  },
  methods: {},
};
</script>

<template>
  <div class="container">
    <start-screen></start-screen>
  </div>
</template>

<style scoped lang="css">
.container {
  display: flex;
  height: 100vh;
  margin: 0 auto;
  max-width: 80vw;
  padding: 40px 20px;
}
</style>
