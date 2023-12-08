<template>
  <div class="wrapper">
    <h1>POKE MEMORIES</h1>
    <p>Select mode to start game</p>
    <div class="modes">
      <button-mode
        v-for="(item, index) of modes"
        :key="index"
        :title="item.title"
        :description="item.description"
      />
    </div>
  </div>
</template>

<script lang="ts">
import { modes } from "../constants/modes";
import Button from "../components/Button.vue";
export default {
  components: {
    ButtonMode: Button,
  },
  data() {
    return {
      modes,
    };
  },
};
</script>

<style scoped lang="css">
.wrapper {
  display: flex;
  width: 100%;
  flex-direction: column;
  justify-content: center;
}
h1 {
  font-size: 40px;
  font-weight: bold;
  line-height: 40px;
  text-align: center;
}
p {
  text-align: center;
  padding: 10px 0px;
  font-size: 24px;
  line-height: 28px;
  font-weight: bold;
}

.modes {
  padding-top: 20px;
  display: flex;
  justify-content: center;
  gap: 20px;
}
</style>
