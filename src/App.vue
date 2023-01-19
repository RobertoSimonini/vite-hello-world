<script>
import AppTitle from  './components/AppTitle.vue';
import AppHero from './components/AppHero.vue';
export default {
  data() {
    return {
  
    }
  }, 
  components: {
    AppTitle,
    AppHero
  }

}
</script>



<template>
<app-title></app-title>
<app-hero></app-hero>
</template>

<style>
img {
  height: 350px;
}
</style>