<template lang="pug">
.container
  v-row
    v-col(row=12)
      PostBlock
  v-row
    v-col(row=12, md=6)
      PostBlock
    v-col(row=12, md=6)
      PostBlock
  v-row
    v-col(row=12, md=4)
      PostBlock
    v-col(row=12, md=4)
      PostBlock
    v-col(row=12, md=4)
      PostBlock
  GptAd(ad-unit='Travel/Europe/France/Paris', :size='[300, 250]')
  //- GptAd(ad-unit='MM_300x600_Sidebar', :size='[600, 300]')
</template>

<script>
import { PostBlock } from '../components'
export default {
  layout: 'main',
  components: { PostBlock },
}
</script>
