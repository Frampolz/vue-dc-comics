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
      src: string,
      alt: string,
      titolo: string
      
    }
}
</script>

<style>

</style>