<template>
  <v-app class="app">
    <router-view name="navbar"></router-view>
    <v-main>
      <router-view name="home"></router-view>
      <router-view name="features"></router-view>
      <router-view name="homeru"></router-view>
      <router-view name="featuresru"></router-view>
      <router-view name="footer"></router-view>
    </v-main>
    <router-view />
  </v-app>
</template>

<script>
export default {
  data: () => ({
  }),
  
};
</script>
