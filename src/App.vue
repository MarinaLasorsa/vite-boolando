<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import axios from 'axios';
import { store } from './store.js';

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  },
  data() {
    return {
      store
    }
  },
  methods: {
    fetchProducts() {
      axios.get('http://localhost:3000/products').then((response) => {
        this.store.products = response.data;
      })
    }
  },
  created: function () {
    this.fetchProducts()
  }
}
</script>

<template>
  <div>
    <AppHeader />
    <AppMain />
    <AppFooter />
  </div>
</template>

<style lang="scss">
@use './styles/general';
</style>