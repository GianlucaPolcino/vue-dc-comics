<template>
  <footer>
      <div class="upper">
          <div class="container">
              <div class="list">
                  <div class="wrapper">
                      <div class="list-links">
                          <h2>
                              DC COMICS
                          </h2>
                          <ul>
                              <li v-for="item in listOne" :key="item.id">
                                  <a href="">{{item.text}}</a>
                              </li>
                          </ul>
                          <h2 class="last-list">
                              SHOP
                          </h2>
                          <ul>
                              <li v-for="item in listFour" :key="item.id">
                                  <a href="">{{item.text}}</a>
                              </li>
                          </ul>
                      </div>
                      <div class="list-links">
                          <h2>
                              DC
                          </h2>
                          <ul>
                              <li v-for="item in listTwo" :key="item.id">
                                  <a href="">{{item.text}}</a>
                              </li>
                          </ul>
                      </div>
                      <div class="list-links">
                          <h2>
                              SITES
                          </h2>
                          <ul>
                              <li v-for="item in listThree" :key="item.id">
                                  <a href="">{{item.text}}</a>
                              </li>
                          </ul>
                      </div>
                  </div>
              </div>
          </div>
      </div>
      <div class="bottom">
          <div class="container">
              <div class="flex">
                  <div>
                      <button>SIGN UP NOW!</button>
                  </div>
                  <div class="flex-2">
                      <h3>FOLLOW US</h3>
                      <a href=""><img src="../assets/img/footer-facebook.png" alt=""></a>
                      <a href=""><img src="../assets/img/footer-twitter.png" alt=""></a>
                      <a href=""><img src="../assets/img/footer-youtube.png" alt=""></a>
                      <a href=""><img src="../assets/img/footer-pinterest.png" alt=""></a>
                      <a href=""><img src="../assets/img/footer-periscope.png" alt=""></a>
                  </div>
              </div>
          </div>
      </div>
  </footer>
</template>

<script>
export default {
    name: "Footer",
    data(){
        return{
            listOne:[
                {
                    id: 0,
                    text: 'Characters',
                },
                {
                    id: 1,
                    text: 'Comics',
                },
                {
                    id: 2,
                    text: 'Movies',
                },
                {
                    id: 3,
                    text: 'TV',
                },
                {
                    id: 4,
                    text: 'Games',
                },
                {
                    id: 5,
                    text: 'Videos',
                },
                {
                    id: 6,
                    text: 'News',
                },
            ],
            listTwo:[
                {
                    id:7,
                    text: 'Term of use',
                },
                {
                    id:8,
                    text: 'Privacy policy (New)',
                },
                {
                    id:9,
                    text: 'Ad Choices',
                },
                {
                    id:10,
                    text: 'Advertising',
                },
                {
                    id:11,
                    text: 'Jobs',
                },
                {
                    id:12,
                    text: 'Subscriptions',
                },
                {
                    id:13,
                    text: 'Talent Workshops',
                },
                {
                    id:14,
                    text: 'CPSC Certificates',
                },
                {
                    id:15,
                    text: 'Ratings',
                },
                {
                    id:16,
                    text: 'Shop help',
                },
                {
                    id:17,
                    text: 'Contact Us',
                },
            ],
            listThree:[
                {
                    id:18,
                    text: 'DC',
                },
                {
                    id:19,
                    text: 'MAD Magazine',
                },
                {
                    id:20,
                    text: 'DC Kids',
                },
                {
                    id:21,
                    text: 'DC Universe',
                },
                {
                    id:22,
                    text: 'DC Power Visa',
                },
            ],
            listFour:[
                {
                    id:23,
                    text: 'Shop DC'
                },
                {
                    id:24,
                    text: 'Shop DC Collectibles'
                },
            ]
        }
    }
}
</script>

<style lang="scss">
    @import "../assets/style/vars.scss";

    .upper{
        background-image: url(../assets/img/footer-bg.jpg);

        .list{
            display: flex;
            background-image: url(../assets/img/dc-logo-bg.png);
            background-position: right;
            background-repeat: no-repeat;
            width: 100%;

            .wrapper{
                width: 60%;
                display: flex;
                flex-wrap: wrap;
                flex-direction: row;
                justify-content: start;
                .list-links{
                    padding-top: 30px;
                    margin-right: 50px;
                    margin-bottom: 30px;

                    h2{
                    color: white;
                    padding-bottom: 10px;
                    font-weight: bold;
                    }

                    ul{
                        list-style: none;

                        li a{
                            text-decoration: none;
                            color: lightgray;

                            &:hover{
                                color: $blue-dc;
                            }
                        }
                    }

                    .last-list{
                        padding-top: 20px;
                    }
                }
            }
            
        }
    }

    .bottom{
        height: 120px;
        background-color: #333333;

        .flex{ 
            width: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            
            button{
            background-color: #333333;
            padding: 16px;
            border: 3px solid $blue-dc;
            color: white;
            font-weight: bold;
            cursor: pointer;

            &:hover{
                background-color: $blue-dc;
            }

            }

            .flex-2{
                display: flex;
                align-items: center;
                
                h3{
                    display: inline-block;
                    margin-right: 20px;
                    color: $blue-dc;
                }

                img{
                    width: 64px;
                    padding: 0 8px;
                }
            }

            
        }
    }
</style>