<template>
  <v-app>

    <app-bar @drawer="changeDrawer" title="App" />
    <app-nav :isActive="drawer" />

    <v-main>
      <router-view/>
    </v-main>

  </v-app>
</template>

<script>
import AppBar from '@/components/AppBar';
import AppNav from '@/components/AppNav';

export default {
  name: 'App',

  components: {
    AppBar, AppNav,
  },

  data() {
    return {
      drawer: false,
    }
  },

  methods: {
    changeDrawer() {
      this.drawer = !this.drawer;
    },
  },

};
</script>
