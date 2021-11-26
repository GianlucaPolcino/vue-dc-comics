<template>
  <div class="card">
      <img :src="card.thumb" :alt="card.series">
      <h5>{{card.series}}</h5>
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
        padding: 8px;

        img{
            width: 100%;
            height: 120px;
            object-fit: cover;
            object-position: top;
        }

        h5{
            padding-top: 6px;
            color: white;
        }
    }
</style>