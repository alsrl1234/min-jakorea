<template>
  <HeaderMenu></HeaderMenu>
  <SlideContent v-bind:SlideData="SlideFrom"></SlideContent>
</template>

<script>
import HeaderMenu from "./components/HeaderMenu.vue";
import SlideContent from "./components/SlideContent.vue";

import SlideTo from "./data/01mainSlide.js";
export default {
  components: {
    HeaderMenu,
    SlideContent,
  },
  data() {
    return {
      SlideFrom: SlideTo,
    };
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}

li {
  list-style: none;
}
a:visited,
a:link {
  text-decoration: none;
  color: #333;
}
a:hover {
  color: #333 !important;
}
</style>