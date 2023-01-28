<template>
  <div class="home">
<div class="splash-container">
        <div class="splash">
          <h1>Splendid Food</h1>
        </div>
      </div>

      <main class="wrapper">
        <h2>Recommended</h2>

        <div class="card-container">
          <ProductCard
          v-for="(product, index) in inventory.slice(0,6)"
            :key="product.id"
            class="card"
            :index="index"
            :product="product"
            :addToCart="addToCart"
          />
        </div>
      </main>

  </div>
</template>

<script>
import ProductCard from '@/components/ProductCard.vue'

// @ is an alias to /src
export default {
  name: 'HomeView',
  props: ['inventory', 'addToCart', 'product'],
  components: {
    ProductCard
  }
}
</script>
