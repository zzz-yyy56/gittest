<template>
  <div id="product-List-two">
    <h2>Product List Two</h2>
    <ul>
        <li v-for="(value,key) in products">
            <span class="name">{{value.name}}</span>
            <span class="price">{{value.price}}</span>
        </li>
    </ul>
  </div>
</template>

<script>
export default {
  props:["products"],
  data () {
    return {
     
    }
  }
}
</script>

<style scoped>
#product-List-two{
    background: #D1E4FF;
    box-shadow: 1px 2px 3px rgba(0,0,0,0.2);
    margin-bottom: 30px;
    padding: 10px 20px;
}
#product-List-two ul{
    padding:0;
    list-style-type: none;
}
#product-List-two li{
    margin-right: 10px;
    margin-top: 10p;
    padding: 20px;
    background: rgba(255, 255, 255, 0.7);
}
.price{
    font-weight: bold;
    color: #860CE8;
    display: block;
}

</style>
