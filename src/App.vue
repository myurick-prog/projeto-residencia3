<template>
  <v-app>
    <router-view></router-view>
  </v-app>
</template>

<script>
export default {
  name: 'App',
  created() {
    this.$store.dispatch('checkAuthState');
  }
}
</script>