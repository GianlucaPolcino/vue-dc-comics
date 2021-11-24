<template>
  <div class="background">
      <div class="container">
          <div class="flex">
              <div class="flex">
                  <img class="img-section" src="../assets/img/buy-comics-digital-comics.png" alt="digital-comics">
                  <span>DIGITAL COMICS</span>
              </div>
              <div class="flex">
                  <img class="img-section" src="../assets/img/buy-comics-merchandise.png" alt="merchandise">
                  <span>DC MERCHANDISE</span>
              </div>
              <div class="flex">
                  <img class="img-section" src="../assets/img/buy-comics-subscriptions.png" alt="subscriptions">
                  <span>SUBSCRIPTION</span>
              </div>
              <div class="flex">
                  <img class="img-section" src="../assets/img/buy-comics-shop-locator.png" alt="shop-location">
                  <span>COMIC SHOP LOCATOR</span>
              </div>
              <div class="flex">
                  <img class="img-section" src="../assets/img/buy-dc-power-visa.svg" alt="power-visa">
                  <span>DC POVER VISA</span>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "Section",
}
</script>

<style lang="scss">    
    @import "../assets/style/vars.scss";

    .background{
        background-color: $blue-dc;
        height: 160px;

        .flex{
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0 auto;
            color: white;
            font-size: 14px;

            .img-section{
                width: 40px;
                height: 100%;
                margin:0 20px;
            }
            
        }
    }
</style>