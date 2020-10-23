<template>
  <div>
    <Introduction id="home"/>
    <OriginalWebsite id="original" />
    <Redesign id ="redesign"/>
    <LoFi id = "lo-fi" />
    <HiFi id = "hi-fi" />
    <VisualStyleGuide id= "visual"/>
    <Deploy id = "redesigned"/>
  </div>
</template>

<script>
import Introduction from './components/Introduction.vue'
import Redesign from './components/Redesign.vue'
import OriginalWebsite from './components/OriginalWebsite.vue'
import LoFi from './components/LoFi.vue'
import HiFi from './components/HiFi.vue'
import VisualStyleGuide from './components/VisualStyleGuide.vue'
import Deploy from './components/Deploy.vue'

export default {
  name: 'App',
  components: {
    Introduction,
    Redesign,
    OriginalWebsite,
    LoFi,
    HiFi,
    VisualStyleGuide,
    Deploy
  }
}
</script>

<style>
</style>
