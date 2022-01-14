<template>
  <div
   class="card-thumbs"
   >
    <img
     :src="src"
     :alt="alt"
     >
    <h3>{{ titolo }}</h3>
  </div>
</template>

<script>
export default {
    name: "Card",
    props:{
      src: String,
      alt: String,
      titolo: String
      
    },
    data() {
      return {

      }
    }
}
</script>

<style>

</style>