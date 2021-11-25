<template>
   <div class="jumbo-bg">
       <div class="series">
           <h2>CURRENT SERIES</h2>
       </div>
   </div>
</template>

<script>
export default {
    name: "Jumbotron"
}
</script>

<style lang="scss" scoped>
    @import "../assets/style/vars.scss";

    .jumbo-bg{
        position: relative;
        background-image: url(../assets/img/jumbotron.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        height: 450px;

        .series{
            position: absolute;
            bottom: -26px;
            left: 190px;
            background-color: $blue-dc;
            padding: 10px;

            h2{
                color: white;
            }
        }
    }
</style>