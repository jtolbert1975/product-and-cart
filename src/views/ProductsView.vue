<template>
    <main className="wrapper">
        <h1>Products</h1>
        <div className="card-container">
            <ProductCard
          v-for="(product, index) in inventory.slice(0,9)"
            :key="product.id"
            class="card"
            :index="index"
            :product="product"
            :addToCart="addToCart"
          />
        </div>
      </main>
</template>

<script>
import ProductCard from '@/components/ProductCard.vue'
export default {
  props: ['inventory', 'addToCart'],
  components: {
    ProductCard
  }
}
</script>
