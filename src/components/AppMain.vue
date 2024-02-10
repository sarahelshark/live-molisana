<script>
import ProductCard from './ProductCard.vue';

export default {
    name: "AppMain",
    data() {
        return {
            products: [
                {
                    src: "https://picsum.photos/400/200",
                    text: "Pasta name 1",
                },
                {
                    src: "https://picsum.photos/400/200",
                    text: "Pasta name 2",
                },
                {
                    src: "https://picsum.photos/400/200",
                    text: "Pasta name 3",
                },
            ],
        };
    },
    components: { ProductCard }
};
</script>

<template>
  <main>
    <section class="products">
      <div class="container">
        <div class="row">
          <div class="col" v-for="product in products">
            <ProductCard :product="product"></ProductCard> <!--props products pr passare costante nella componente -->
          </div>

        </div>
        
      </div>
    </section>
  </main>
</template>

<style scoped>
main {
  min-height: 400px;
  background-image: url("/img/fondo-pag-speciali.jpg");
  filter: opacity(90%);
}
</style>
