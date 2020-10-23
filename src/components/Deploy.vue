<template>
  <div>
    <b-jumbotron fluid container-fluid="md" bg-variant="white" border-variant="dark" class="full-height">
      <template #header>Deploying Homepage</template>

      <template #lead>
        As a final step using the final high-fidelity prototypes, I created the homepage using HTML and CSS! This final website is responsive 
        and was also testing for accessibility. When tabbing through the content the expected content order follows the visual order of the page reading.
        This order starts with the header, followed by the main navigation, page navigation, main content, and finally the footer. Within those segments of the
        page, the related content is grouped together. The buttons have visual focus and are highlighted on hover. 
      </template>


      <b-container class="bv-example-row">
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light"></p>
            <b-img height="400px" width="800px"  :src="require('../assets/deploy.png')" fluid alt="Responsive image"></b-img>
            <p class="mt-4 h5 font-weight-light text-center">Redesigned Homepage</p>
          </b-col>
        </b-row>
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light"></p>
            <b-img height="200px" width="200px"  :src="require('../assets/responsive tab.png')" fluid alt="Responsive image"></b-img>
            <p class="mt-4 h5 font-weight-light text-center">Responsive on Tablet</p>
          </b-col>
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light"></p>
            <b-img height="200px" width="200px"  :src="require('../assets/responsive mobile.png')" fluid alt="Responsive image"></b-img>
            <p class="mt-4 h5 font-weight-light text-center">Responsive on Mobile</p>
          </b-col>
        </b-row>
        <b-row style="border: 1px solid">
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light"></p>
            <b-img height="200px" width="400px"  :src="require('../assets/large2.png')" fluid alt="Responsive image"></b-img>
          </b-col>
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light"></p>
            <b-img height="200px" width="400px"  :src="require('../assets/large3.png')" fluid alt="Responsive image"></b-img>
          </b-col>
        </b-row>
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light"></p>
            <b-img height="200px" width="400px"  :src="require('../assets/large4.png')" fluid alt="Responsive image"></b-img>
          </b-col>
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light"></p>
            <b-img height="200px" width="400px"  :src="require('../assets/large5.png')" fluid alt="Responsive image"></b-img>
          </b-col>
        </b-row>
        </b-row>
            <p class="mt-4 h5 font-weight-light text-center">Also works for large font size</p>

        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light"></p>
            <b-img height="200px" width="300px"  :src="require('../assets/mywave.png')" fluid alt="Responsive image"></b-img>
            <p class="m-4 h5 font-weight-light text-center">Wave Accessibility Report</p>
          </b-col>
        </b-row>
      </b-container>

      <div class="text-center">
      <b-button variant="info" class="ml-2" size="lg"  href="https://frozen-basin-88210.herokuapp.com/" >DEPLOYED HOMEPAGE</b-button>
        <b-button class="m-5" variant="success" href="#" size="lg" v-scroll-to="'#home'">BACK TO HOME</b-button>
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
