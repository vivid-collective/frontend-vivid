
<template>
  <div>
    <carousel></carousel>
    <section style="height: 50vh">
      <h2>“We make super comfy sunglasses that fit like a glove and won’t slide around when you’re doing fun stuff. Every pair sold supports the environment and won’t break the bank in the process.”</h2>
    </section>
    <image-collection></image-collection>
  </div>
</template>

<script>
  import carousel from './Carousel.vue'
  import imageCollection from './ImageCollection.vue'
  export default {
    name: "landingPage",
    components: {
      carousel,
      imageCollection
    }
  }

</script>
<style scoped style lang="scss">

</style>
