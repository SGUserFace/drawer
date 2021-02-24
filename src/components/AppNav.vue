<template>
  <div>

    <v-navigation-drawer :value="isActive" app fixed temporary></v-navigation-drawer>

  </div>
</template>

<script>
export default {

  name: 'AppNav',

  props: [
    'isActive',
  ],

}
</script>
