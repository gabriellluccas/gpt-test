<template lang="pug">
v-app(dark)
  LayoutNavbar
  v-main
    v-container
      nuxt
  LayoutFooter
</template>

<script>
import { LayoutNavbar, LayoutFooter } from '../components'
export default {
  components: { LayoutNavbar, LayoutFooter },
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
    }
  },
}
</script>
