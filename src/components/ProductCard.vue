<script>
export default {
  name: "ProductCard",
  props: {
    src:String,
    text:String, 
  }
};
</script>
<template>
  <div class="product">
    <img :src='src' alt=''/>
    <h3>{{ text}}</h3>
  </div>
</template>
<style></style>
