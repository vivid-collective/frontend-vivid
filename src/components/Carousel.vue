
<template>
  <v-carousel hide-delimiters style="height: 100vh">
    <v-carousel-item
    v-for="(photo,i) in photos"
    :src="photo.src"
    :key="i"
    >
    </v-carousel-item>
  </v-carousel>
</template>

<script>
export default {
  name: "carousel",
  data() {
    return {
      photos: [
        {
          src: "/static/paul.jpg"
        },
        {
          src: "/static/paul.jpg"
        },
        {
          src: "/static/paul.jpg"
        },
        {
          src: "/static/paul.jpg"
        }
      ]
    };
  }
};
</script>
<style scoped style lang="scss">

</style>
