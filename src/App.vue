<template>
  <HeaderMenu></HeaderMenu>
  <SlideContent></SlideContent>
</template>

<script>

import HeaderMenu from "./components/HeaderMenu.vue"
import SlideContent from "./components/SlideContent.vue"
export default {
    components:{
        HeaderMenu,
        SlideContent
    },

}
</script>

<style>
 *{margin: 0;padding: 0;}

 li{
  list-style: none;
 }
 a:visited,a:link{
  text-decoration: none;
  color: #333;
 }
 a:hover{
  color: #333;
 }
</style>