<template lang="html">
  <div class="">
    <app-stock v-for="stock in stocks"></app-stock>
  </div>
</template>

<script>
import Stock from './Stock.vue';
export default {
  data() {
    return {
      stocks: [
        { id: 1, name: 'BMW', price: 110},
        { id: 2, name: 'Tesla', price: 120},
        { id: 3, name: 'Apple', price: 130},
        { id: 4, name: 'Baidu', price: 140},
      ]
    }
  },
  components: {
    appStock: Stock
  }
}
</script>

<style lang="css" scoped></style>
