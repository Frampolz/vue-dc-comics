<template>
<footer>
    <div class="footer-top">
        <div class="footer-top-container container d-flex">
            <div class="footer-list d-flex">
                <div class="list-left">
                <ul>
                    <h2>dc comics</h2>
                    <li><a href="#">character</a></li>
                    <li><a href="#">comics</a></li>
                    <li><a href="#">movies</a></li>
                    <li><a href="#">tv</a></li>
                    <li><a href="#">games</a></li>
                    <li><a href="#">videos</a></li>
                    <li><a href="#">news</a></li>
                </ul>
                <ul>
                    <h2>shop</h2>
                    <li><a href="#">shop dc</a></li>
                    <li><a href="#">shop dc collectibles</a></li>

                </ul>
                </div>
                <div class="right-list d-flex">
                <ul>
                    <h2>dc</h2>
                    <li><a href="#">terms of use</a></li>
                    <li><a href="#">privacy policy (new)</a></li>
                    <li><a href="#">ad choices</a></li>
                    <li><a href="#">advertising</a></li>
                    <li><a href="#">jobs</a></li>
                    <li><a href="#">subscription</a></li>
                    <li><a href="#">talent workshops</a></li>
                    <li><a href="#">cpsc certificates</a></li>
                    <li><a href="#">ratings</a></li>
                    <li><a href="#">shop help</a></li>
                    <li><a href="#">contact us</a></li>
                </ul>
                <ul>
                    <h2>sites</h2>
                    <li><a href="#">dc</a></li>
                    <li><a href="#">mad magazine</a></li>
                    <li><a href="#">dc kids</a></li>
                    <li><a href="#">dc universe</a></li>
                    <li><a href="#">dc visa</a></li>
                </ul>
                </div>
            </div>
            <div class="footer-top-logo d-flex">
               <img src="../assets/img/dc-logo-bg.png" alt="">

            </div>
        </div>
    </div>
    <div class="footer-bot">
        <div class="footer-bot-container container d-flex">
            <div class="button">
                <a href="">sign-up now!</a>
            </div>
            <div class="contact-list">
                    <ul class="d-flex">
                        <li>
                            <h2>follow us</h2>
                        </li>
                        <li>
                            <a href="#">
                            <img src="../assets/img/footer-facebook.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                            <img src="../assets/img/footer-twitter.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                            <img src="../assets/img/footer-youtube.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                            <img src="../assets/img/footer-pinterest.png" alt="">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                            <img src="../assets/img/footer-periscope.png" alt="">
                            </a>
                        </li>
                    </ul>
            </div>
        </div>
    </div>
</footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";
footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    
.footer-top {
    
        .footer-top-container{
            justify-content: space-between;
            text-align: left;
            
            .footer-list {
                align-items: flex-start;
                ul {
                    margin-right: 2em;
                }

                h2 {
                    margin-bottom: 0.5em;
                }
                
                a {
                    color: gray;
                    font-size: 0.8em;
                    text-transform: capitalize;
                }
                .list-left {
                    ul:first-of-type {
                        margin-bottom: 1.5em;
                    }
                }
                .right-list {
                    align-items: flex-start;
                }
            }
        }
        .footer-top-logo { 
            height: 370px;
            overflow: hidden;
        } 
    }
    .footer-bot {
        background-color: $footerBotBg;
        text-transform: uppercase;

        .footer-bot-container {
            justify-content: space-between;

            .button {
                a {
                    color: white;
                    border: 2px solid $blueColor;
                    padding: 1em;
                }
            }
            ul {
                padding: 2.5em;

                li {
                    display: inline-block;
                    padding: 0.5em;

                h2 {
                    color: $blueColor
                }

                }
            } 
        }
    }
}

</style>