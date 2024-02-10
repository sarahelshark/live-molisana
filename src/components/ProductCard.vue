<script>
export default {
  name: "ProductCard",
  props: {
    /*props:['product'],*/
    product: Object
  }
};
</script>
<template>
  <div class="product">
    <img :src="product.src" alt="random img" />
    <h3>{{ product.text }}</h3>
  </div>
</template>
<style></style>
