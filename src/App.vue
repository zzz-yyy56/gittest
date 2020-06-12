<template>
  <div id="app">
    <product-List-one v-bind:products="products"></product-List-one>
    <product-List-two v-bind:products="products"></product-List-two>  
  </div>
</template>

<script>
import productListOne from './components/productListOne'
import productListTwo from './components/productListTwo'
export default {
  name: 'app',
  data () {
    return {
      
    }
  },
  components:{
    'product-List-one':productListOne,
    'product-List-two':productListTwo,
  }
}
</script>

<style>
body{
  font-family:Ubuntu;
  color:#555;
}

</style>
