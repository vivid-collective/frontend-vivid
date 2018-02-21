<template>
  <v-app>
    <v-layout justify-space-between>
      <div id="main-logo"><Logo></Logo></div>
      <nav id="top-right-nav-icons">
        <div class="icon"><Person></Person></div>
        <div class="icon"><Cart></Cart></div>
        <div @click.stop="drawer = !drawer" class="icon">
          <Hamburger></Hamburger>
        </div>
      </nav>
      <v-navigation-drawer
        temporary
        v-model="drawer"
        absolute
        right
      >
      <v-list class="pa-1">
        <v-list-tile avatar>
          <v-list-tile-avatar>
            <img src="https://randomuser.me/api/portraits/men/85.jpg" >
          </v-list-tile-avatar>
          <v-list-tile-content>
            <v-list-tile-title>John Leider</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
      <v-list class="pt-0" dense>
        <v-divider></v-divider>
        <v-list-tile v-for="item in items" :key="item.title">
          <v-list-tile-action>
            <!-- <v-icon>{{ item.icon }}</v-icon> -->
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>{{ item.title }}</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
      </v-navigation-drawer>
    </v-layout>
  </v-app>
</template>

<script>
import Hamburger from "../assets/svg/hamburger.svg";
import Person from "../assets/svg/person.svg";
import Cart from "../assets/svg/cart.svg";
import Logo from "../assets/svg/logo.svg";

export default {
  name: "navigation",
    components: {
    Hamburger,
    Person,
    Cart,
    Logo
  },
  data () {
      return {
        drawer: null,
        items: [
          { title: 'Home', icon: 'dashboard' },
          { title: 'About', icon: 'question_answer' }
        ]
      }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped style lang="scss">
#main-logo{
  padding: 2em 4em;
}
#top-right-nav-icons {
  padding: 2em;
  .icon {
    margin: 1em
  };
}
</style>
