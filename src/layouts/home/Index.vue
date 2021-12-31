<template>
  <v-app>
    
    <home-app-bar />

    <home-view />

    <home-footer />

    <home-settings />

    <home-secondary-menu />

    

  </v-app>
</template>

<script>
  export default {
    name: 'HomeLayout',

    components: {
      HomeAppBar: () => import('@/layouts/home/AppBar'),
      HomeFooter: () => import('@/layouts/home/Footer'),
      HomeSettings: () => import('@/layouts/home/Settings'),
      HomeMenu: () => import('@/layouts/home/menu'),
      HomeSecondaryMenu: () => import('@/layouts/home/SecondaryMenu'),
      HomeView: () => import('@/layouts/home/View'),
    },
  }
</script>
