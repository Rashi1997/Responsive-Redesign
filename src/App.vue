<template>
  <div>
    <Introduction />
    <OriginalWebsite id="original" />
    <Redesign id ="redesign"/>
    <LoFi id = "lo-fi" />
    <HiFi id = "hi-fi" />
  </div>
</template>

<script>
import Introduction from './components/Introduction.vue'
import Redesign from './components/Redesign.vue'
import OriginalWebsite from './components/OriginalWebsite.vue'
import LoFi from './components/LoFi.vue'
import HiFi from './components/HiFi.vue'

export default {
  name: 'App',
  components: {
    Introduction,
    Redesign,
    OriginalWebsite,
    LoFi,
    HiFi
  }
}
</script>

<style>
</style>
