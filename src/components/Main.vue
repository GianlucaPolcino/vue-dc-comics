<template>
  <div class="main-bg">
      <div class="container">
          <div class="card-flex">
              <Product
              v-for="(card, index) in cards"
              :key="index"
              :card="card"
               />
          </div>
      </div>
  </div>
</template>

<script>
import cards from "../assets/data/productData.js";
import Product from "./Product.vue"

export default {
    name: "Main",
    components: {
        Product
    },

    data(){
        return{
            cards,
        }
    }
}
</script>

<style lang="scss">
    .main-bg{
        background-color: #222222;

        .card-flex{
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-items: center;
            padding: 34px 0;
            margin: 0 auto;
        }
    }
</style>