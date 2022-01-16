<template>
<main>
    <div class="jumbotron">
        <img src="../assets/img/jumbotron.jpg" alt="">
  </div>
    <div class="container">
        <div class="current-box">
            <h2>current series</h2>
        </div>
        <Cardmain />
      </div>
      
      
  <div class="main-link">
      <ul class="d-flex">
<!--           <li v-for="(icone, index) in iconList" :key="index">
              <a href="">
                <img :src="`../assets/img/${icone.src}`" alt="">
                <p>{{icone.text}}</p>
              </a>
          </li> -->
          <li><a href="">
              <div class="icon-box">
              <img src="../assets/img/buy-comics-digital-comics.png" alt="">   
              </div>
              <p>digital comics</p>       
            </a>
            </li>
          <li><a href="">
              <div class="icon-box">
              <img src="../assets/img/buy-comics-merchandise.png" alt="">  
              </div> 
              <p>dc merchandise</p>       
            </a>
            </li>
          <li><a href="">
              <div class="icon-box">
              <img src="../assets/img/buy-comics-subscriptions.png" alt="">   
              </div>
              <p>subscription</p>       
            </a>
            </li>
          <li><a href="">
              <div class="icon-box">
              <img src="../assets/img/buy-comics-shop-locator.png" alt=""> 
              </div>  
              <p>comic shop locator</p>       
            </a>
            </li>
          <li><a href="">
              <div class="icon-box">
              <img src="../assets/img/buy-dc-power-visa.svg" alt="">   
              </div>
              <p>dc power visa</p>       
            </a>
            </li>
      </ul>
  </div>
</main>
</template>

<script>
import Cardmain from './Cardmain.vue';


export default {
    data() {
        return {
            iconList: [
                {
                    src: "buy-comics-digital-comics.png",
                    text: "digital comics"
                },
                {
                    src: "buy-comics-merchandise.png",
                    text: "dc merchandise"
                },
                {
                    src: "buy-comics-subscriptions.png",
                    text: "subscription"
                },
                {
                    src: "buy-comics-shop-locator.png",
                    text: "comic shop locator"
                },
                {
                    src: "buy-dc-power-visa.svg",
                    text: "dc power visa"
                }
            ]
        }
    },
    components: {
        Cardmain,
        
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";
main {
    background-color: $mainBgColor;

        .jumbotron {
            height: 400px;
            overflow: hidden;
            
        }

        .container {
            position: relative;

            .current-box {
                position: absolute;
                top: -5em;
                left: 0;
                background-color: $blueColor;
                padding: 0.5em 1em;
            }
        }
        
        .main-link {
            background-color: $blueColor;
            ul {
                justify-content: center;

            
             li {
                display: inline-block;
                padding: 3em 3.5em;

                a {
                    display: flex;
                    flex-direction: row;
                    text-decoration: none;
                    justify-content: center;
                    align-items: center;
                    .icon-box {
                        width: 40px;
                        height: 50px;
                        margin-right: 1em;
                        img {
                            height: 100%;
                            
                        }
                        
                        

                    }
                    p {
                        color: white;
                    }
                }
            }
            & li:last-child a .icon-box {
                width: 30%;
                img {
                    width: 100%;
                }
            }
        }
        }
}
</style>