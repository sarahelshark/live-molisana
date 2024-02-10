<script>
export default {
  name: "ProductCard",
  props: {
    /*props:['product'],*/
    product: Object,
    /*src:String,
    text:String,  opzione 2 */
  }
};
</script>
<template>
  <div class="product">
    <img :src="product.src" alt="random img" />
    <h3>{{ product.text }}</h3>
    <!--opzione 2 
     <img :src='src' alt=''/>>
    <h3>{{ text
    -->
  </div>
</template>
<style></style>
