<template>
  <nav id="landing-page">
    <h1>Landing Page</h1>
    <SomeIcon class="icon"/>
  </nav>
</template>

<script>
import SomeIcon from "../assets/svg/most-recent-logo.svg";

export default {
  name: "landing-page",
  components: {
    SomeIcon
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped style lang="scss">
.icon {
  width: 100vh;
}
</style>
