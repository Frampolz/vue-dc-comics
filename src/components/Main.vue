<template>
<main>
    <div class="jumbotron">
        <img src="../assets/img/jumbotron.jpg" alt="">
  </div>
    <div class="container">
        <Cardmain />
      </div>
      
      
  <div class="main-link">
      <ul class="d-flex">
          <li><a href="">
              <img src="../assets/img/buy-comics-digital-comics.png" alt="">   
              <p>digital comics</p>       
            </a>
            </li>
          <li><a href="">
              <img src="../assets/img/buy-comics-merchandise.png" alt="">   
              <p>dc merchandise</p>       
            </a>
            </li>
          <li><a href="">
              <img src="../assets/img/buy-comics-subscriptions.png" alt="">   
              <p>subscription</p>       
            </a>
            </li>
          <li><a href="">
              <img src="../assets/img/buy-comics-shop-locator.png" alt="">   
              <p>comic shop locator</p>       
            </a>
            </li>
          <li><a href="">
              <img src="../assets/img/buy-dc-power-visa.svg" alt="">   
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
                    img {
                        width: 40px;
                        margin-right: 0.5em;
                    }
                    p {
                        color: white;
                    }
                }
            }
        }
        }
}
</style>