<template>
  <div>

    <v-app-bar fixed app>
	  <v-app-bar-nav-icon @click.stop="changeDrawer"></v-app-bar-nav-icon>
      <v-toolbar-title>{{ title }}</v-toolbar-title>
    </v-app-bar>

  </div>
</template>

<script>
export default {

  name: 'AppBar',

  props: {
    title: {
      type: String,
      required: false,
    },
  },

  methods: {
    changeDrawer() {
      this.$emit('drawer');
    },
  },

}
</script>
