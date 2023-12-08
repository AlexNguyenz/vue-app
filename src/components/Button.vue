<template>
  <button>
    <p class="text">{{ title }}</p>
    <p class="text">{{ description }}</p>
  </button>
</template>

<script lang="ts">
export default {
  props: {
    title: String,
    description: String,
  },
};
</script>

<style scoped lang="css">
button {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
  gap: 10px;
  padding: 20px 0;
  border-radius: 10px;
  width: 120px;
  cursor: pointer;
}

.text {
  width: 100%;
  text-align: center;
  font-size: 20px;
  line-height: 24px;
  font-weight: 500;
  white-space: nowrap;
}
</style>
