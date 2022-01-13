<template>
<div class="container d-flex">
    <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <div class="menu">
        <ul>
            <li><a href="#">character</a></li>
            <li><a href="#">comics</a></li>
            <li><a href="#">movie</a></li>
            <li><a href="#">tv</a></li>
            <li><a href="#">games</a></li>
            <li><a href="#">collectibles</a></li>
            <li><a href="#">videos</a></li>
            <li><a href="#">fans</a></li>
            <li><a href="#">news</a></li>
            <li><a href="#">shop</a></li>
        </ul>
    </div>
</div>
</template>

<script>
export default {
data() {
    return {

    }
}
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";

.container {
    justify-content: space-between;
    text-transform: uppercase;
}
img {
    padding: 1em;
}
ul {
    list-style-type: none;
    li {
        display: inline-block;
        padding: 1em;
        &:hover,
        &:active,
        &.active {
            border-bottom: 2px solid $blueColor;
        }

        
        a {
            text-decoration: none;
            
            &:hover,
            &:active,
            &.active {
                color: $blueColor;
            }
        }
    }
}
</style>