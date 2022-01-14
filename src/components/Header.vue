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
    
    li {
        display: inline-block;
        padding: 1em;

        a {
            text-decoration: none;
            padding: 3.8em 0;
            color: $headerLiColor;
            font-weight: bold;
            font-size: 0.9em;
            &:hover,
            &:active,
            &.active {
                color: $blueColor;
                border-bottom: 5px solid $blueColor;
            }
        }
    }
}
</style>