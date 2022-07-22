<script>
export default {
  setup() {
    const buttonClicked = () => {
      console.log('button clicked');
    };

    return { buttonClicked };
  },
};
</script>
<template>
  <button class="poc-button" @click="buttonClicked">
    <slot />
  </button>
</template>

<style scoped>
.poc-button {
  background: #43b883;
  padding: 0.5rem 1rem;
  margin: 1rem;
  color: white;
  outline: none;
  border: none;
  cursor: pointer;
}
</style>
