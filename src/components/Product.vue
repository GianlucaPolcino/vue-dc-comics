<template>
  <div class="card">
      <img :src="card.thumb" :alt="card.series">
      <h4>{{card.series}}</h4>
  </div>
</template>

<script>
export default {
    name: "Product",
    props:{
        card: Object,
    }
}
</script>

<style lang="scss">
    .card{
        flex-basis: 15%;
        padding: 10px;

        img{
            width: 100%;
        }

        h4{
            color: white;
        }
    }
</style>