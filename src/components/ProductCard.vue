<script>
export default {
  name: "ProductCard",
  props: {
    src: String,
    text: String,
  },
};
</script>
<template>
  <div class="product">
    <img :src="src" alt="" />
    <h3>{{ text }}</h3>
  </div>
</template>
<style scoped>
.product {
  background-color: var(--mol-light);
  height: 100%;
  border-radius: 1rem;
  transition: all 1s;
  &:hover {
    filter: drop-shadow(0 0 15px #002d75);
  }

  & img {
    border-top-right-radius: 1rem;
    border-top-left-radius: 1rem;
  }

  & h3 {
    padding: 1rem;
  }
}
</style>
