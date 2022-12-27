<template>
  <div class="my-app">
  <appheader />
  <apphero />
  <appabout />
  </div>
  <router-view/>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import appheader from './components/appheader.vue'
import apphero from './components/apphero.vue'
import appabout from './components/appabout.vue'
export default defineComponent({
 components:  {
  appheader,
  apphero,
  appabout,
 },
  
})
</script>


<style>
body {
    margin: 0;
    background-color: #000000;
}
</style>
