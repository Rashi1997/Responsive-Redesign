<template>
  <div>
    <b-jumbotron fluid container-fluid="md" bg-variant="white" border-variant="dark" class="full-height">
      <template #header>Visual Style Guide</template>

      <template #lead>
      </template>


      <b-container class="bv-example-row">
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light"></p>
            <b-img height="400px" width="800px"  :src="require('../assets/visualstyleguide.png')" fluid alt="Responsive image"></b-img>
            <p class="mt-4 h5 font-weight-light text-center">Style guide for the redesigned website</p>
          </b-col>
        </b-row>
      </b-container>

      <div class="text-center">
        <b-button class="m-5" variant="success" href="#" size="lg" v-scroll-to="'#home'">BACK TO HOME</b-button>
        <b-button class="m-5" variant="success" href="#" size="lg" v-scroll-to="'#redesigned'">DEPLOYING HOMEPAGE</b-button>
      </div>
    
    </b-jumbotron>
  </div>
</template>

<script>

export default {
  name: 'HiFi',
  components: {
  }
}
</script>

<style scoped>
  .full-height {
    padding-bottom: 15rem;
    margin-bottom: 0;
    border: 0!important;
  }
</style>
