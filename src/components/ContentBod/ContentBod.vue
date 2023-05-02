<template>
  <div class="ContentBod__Container">
    <h1 class="ContentBod__Title">{{ title }}</h1>
    <slot></slot>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    title: String
  }
})
</script>

<style lang="sass">
.ContentBod__Container
  display: 'flex'
  flex-direction: 'column'

.ContentBod__Title
  color: 'gray',
  margin-bottom: 15
  font-size: 1rem
</style>
