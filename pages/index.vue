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
  v-row
    v-col(row=12)
      GptAd(ad-unit='/jc_teste_300x250', :size='size')
    //- v-col(row=12)
      //- GptAd(ad-unit='243345435/Travel/Europe/France/Paris', size='300x250')
</template>

<script>
import { PostBlock } from '../components'
export default {
  layout: 'main',
  components: { PostBlock },
  data() {
    return {
      size: [
        [300, 250],
        [728, 90],
        [750, 200],
      ],
    }
  },
}
</script>
