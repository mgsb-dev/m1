<template>
  <header>
    <nav class="NavBar" aria-expanded="false">
      <ul class="NavBar__content">
        <li id="home" class="NavBar__list-title" @click.prevent="goHome">
          <RouterLink to="/" class="NavBar__list-title--dark">Home</RouterLink>
        </li>
        <li
          id="gallery"
          class="NavBar__list-title"
          @click.prevent="goToGallery"
        >
          <RouterLink to="/gallery" class="NavBar__list-title--dark"
            >Gallery</RouterLink
          >
        </li>
      </ul>
    </nav>
  </header>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import { RouterLink } from "vue-router";

export default defineComponent({
  components: { RouterLink },
  setup() {
    const goToGallery = (): void => {
      console.log("gallery");
    };

    const goHome = (): void => {
      console.log("home");
    };

    return {
      goHome,
      goToGallery,
    };
  },
});
</script>

<style lang="sass">
@import './NavBar.sass'
</style>
