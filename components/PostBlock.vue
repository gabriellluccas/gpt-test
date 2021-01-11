<template lang="pug">
v-card.mx-auto
  v-img(
    src='https://cdn.vuetifyjs.com/images/cards/sunshine.jpg',
    :height='heigth'
  )
  v-card-title The title for this post
  v-card-subtitle
    v-card-actions
      v-spacer 

      v-btn(icon) 
        v-icon mdi-heart

      v-btn(icon) 
        v-icon mdi-bookmark

      v-btn(icon) 
        v-icon mdi-share-variant
</template>

<script>
export default {
  props: {
    heigth: {
      type: String,
      default: '200px',
    },
  },
}
</script>
