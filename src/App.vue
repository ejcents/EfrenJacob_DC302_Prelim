<template>
  <div class="app-vue">
    <ItemList :products="products" />
  </div>
</template>

<script>
import ItemList from './components/ItemList.vue'

export default {
  name: 'App',
  components: {
    ItemList
  },
  data() {
    return {
      products: [
        { name: 'Yach', price: 150, visible: true },
        { name: 'Chad', price: 110, visible: true },
        { name: 'Evo', price: 250, visible: true },
        { name: 'Jacob', price: 300, visible: true },
        { name: 'Louie', price: 900, visible: true }
      ]
    }
  }
}
</script>
