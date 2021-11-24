<template>
  <div class="header">
      <div class="container">
          <a href="">
            <img src="../assets/img/dc-logo.png" alt="">
          </a>
          <ul class="nav">
              <li v-for="(item, index) in links" :key="index">
                  <a href="item.url">{{item.text}}</a>
              </li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
    name:"Header",
    data(){
        return{
            links:[
                {
                    url:'/characters',
                    text: 'CHARACTERS',
                    current: false
                },
                {
                    url:'/comics',
                    text: 'COMICS',
                    current: false
                },
                {
                    url:'/movies',
                    text: 'MOVIES',
                    current: false
                },
                {
                    url:'/tv',
                    text: 'TV',
                    current: false
                },
                {
                    url:'/games',
                    text: 'GAMES',
                    current: false
                },
                {
                    url:'/collectibles',
                    text: 'COLLECTIBLES',
                    current: false
                },
                {
                    url:'/videos',
                    text: 'VIDEOS',
                    current: false
                },
                {
                    url:'/fans',
                    text: 'FANS',
                    current: false
                },
                {
                    url:'/news',
                    text: 'NEWS',
                    current: false
                },
                {
                    url:'/shop',
                    text: 'SHOP',
                    current: false
                },
            ]
        }
    }
}

</script>

<style lang="scss">
    .header{
        height: 120px;
        background-color: white;
    }

    
</style>