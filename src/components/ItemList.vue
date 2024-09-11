<template></template>

<script>
import Item from './Item.vue'

export default {
  name: 'ItemList',
  components: {
    Item,
      },
      props: {
        products {
        type: Array,
        required: true
        }
        }
    }
</script>
