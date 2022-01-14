<template>
  <div
   class="card-thumbs"
   >
   <div class="img-box">
    <img
     :src="src"
     :alt="alt"
     >

   </div>
   <div class="title">
    <h3>{{ titolo }}</h3>

   </div>
  </div>
</template>

<script>
export default {
    name: "Card",
    props:{
      src: String,
      alt: String,
      titolo: String
      
    }
}
</script>

<style>
    .img-box {
      height: 200px;
      overflow: hidden;
    }
    h3 {
      text-align: start;
      padding-top: 0.5em;
      font-weight: normal;
      font-size: 1em;
      color: white;
    }
</style>