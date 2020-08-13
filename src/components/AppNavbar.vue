<template>
  
  <v-app-bar
    v-scroll="onScroll"
    :color="!isScrolling ? 'transparent' : 'transparent'"
    fixed
    flat
    dark
  >
    <v-slide-x-transition>
      <v-img
        v-if="showLogo"
        :src="require('@/assets/logo-pitch-match.png')"
        class="shrink"
        contain
        height="50"
        position="relative"
      />
    </v-slide-x-transition>

    <v-spacer />
     <v-btn-toggle
          rounded
          mandatory
        >
          <router-link to="/ru">
            <v-btn icon>
              ru
            </v-btn>
          </router-link>
          <router-link to="/en">
            <v-btn icon>
              en
            </v-btn>
          </router-link>

        </v-btn-toggle>

  </v-app-bar>
</template>

<script>
  export default {
    name: 'AppNavbar',

    data: () => ({
      showLogo: false,
      isScrolling: false,
      
    }),

    methods: {
      onScroll () {
        const offset = window.pageYOffset
        this.isScrolling = offset > 50
        this.showLogo = offset > 200
        
      },
    },
  }
</script>
