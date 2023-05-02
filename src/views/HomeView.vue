<template>
  <div class="HomeView__Container">
    <ContentBod title="You're in the Home section!">
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
.HomeView__Container
  display: 'flex'
  flex-direction: 'column'

.HomeView__Title
  color: 'gray',
  margin-bottom: 15
</style>
