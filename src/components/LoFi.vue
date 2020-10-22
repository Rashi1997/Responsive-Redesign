<template>
  <div>
    <b-jumbotron fluid container-fluid="md" bg-variant="white" border-variant="dark" class="full-height">
      <template #header>Lo-Fi Wireframes</template>

      <template #lead>
        I have sketched the annotated wireframes below for desktop, tablet and mobile. The annotations specify what specific
        feature has been added to uplift the current design.
      </template>
      <b-container class="bv-example-row">
        <b-row align-v="center">
          <b-col class="text-center mt-5 mb-5 ml-3 mr-3">
            <b-img :src="require('../assets/desktop-lo.png')" fluid alt="Responsive image"></b-img>
            <p class="mt-4 h5 font-weight-light">Lo-fi for Desktop</p>
          </b-col>
        </b-row>
        <b-row align-v="center">
          <b-col class="text-center mt-5 mb-5 ml-3 mr-3">
            <b-img :src="require('../assets/tablet-lo.png')" fluid alt="Responsive image"></b-img>
            <p class="mt-4 h5 font-weight-light">Lo-fi for Tablet</p>
          </b-col>
        </b-row>
        <b-row align-v="center">
          <b-col class="text-center mt-5 mb-5 ml-3 mr-3">
            <b-img :src="require('../assets/mobile-lo.png')" fluid alt="Responsive image"></b-img>
            <p class="mt-4 h5 font-weight-light">Lo-fi for Mobile</p>
          </b-col>
        </b-row>
      </b-container>
      <div class="text-center">
        <b-button class="m-5" variant="success" href="#" size="lg" v-scroll-to="'#hi-fi'">HI-FI PROTOTYPE</b-button>
        <b-button class="m-5" variant="success" href="#" size="lg" v-scroll-to="'#redesign'">BACK TO REDESIGN</b-button>
      </div>
    
    </b-jumbotron>
  </div>
</template>

<script>

export default {
  name: 'LoFi',
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
