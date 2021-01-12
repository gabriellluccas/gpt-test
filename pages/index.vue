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
  GptAd(ad-unit='MM_300x600_Sidebar', :size='size')
</template>

<script>
import { PostBlock } from '../components'
export default {
  layout: 'main',
  components: { PostBlock },
  data() {
    return {
      size: ['160x600', '300x600'],
    }
  },
}
</script>
