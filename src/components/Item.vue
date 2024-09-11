<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div v-if="item.isVisible" class="item">
    <h3>{{ item.name }}</h3>
    <p>Price: ${{ item.price.toFixed(2) }}</p>
    <button @click="addToCart">Add to Cart</button>
  </div>
</template>

<script>
export default {
  name: `Item`,
  props: {
    item: {
      type: Object,
      required: true
    }
  },
  methods: {
    addToCart() {
      console.log(`Added to cart: $(this.item.name) - $$(this.item.price)`)
      this.$emit('add-to-cart', this.item)
    }
  }
}
</script>
