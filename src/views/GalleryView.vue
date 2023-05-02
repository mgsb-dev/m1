<template>
  <div class="GalleryView__Container">
    <ContentBod title="You're in the Gallery section!">
      <p>Feel free to explore!</p>
    </ContentBod>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import ContentBod from '@/components/ContentBod/ContentBod.vue'

export default defineComponent({
  props: {
    title: String
  },
  components: { ContentBod }
})
</script>

<style lang="sass">
.GalleryView__Container
  display: 'flex'
  flex-direction: 'column'

.GalleryView__Title
  color: 'gray',
  margin-bottom: 15
</style>
