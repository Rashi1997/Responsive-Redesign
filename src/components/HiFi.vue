<template>
  <div>
    <b-jumbotron fluid container-fluid="md" bg-variant="white" border-variant="dark" class="full-height">
      <template #header>Hi-Fi Wireframes</template>

      <template #lead>
        The Hi-fi prototypes were created and annotated using Figma, with all the hover state and scrolling interactions.
      </template>

      <p class="m-4 h2 font-weight-bold text-center">Hi-fi for Desktop</p>
      <iframe src="https://drive.google.com/file/d/1it-6L1GApfSZ8RSUh5iD-XESxqEAQwl4/preview" width="90%" height="500"></iframe>

      <!-- <b-container class="bv-example-row">
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light">Main Landing Page annotated</p>
            <b-img height="400px" width="800px"  :src="require('../assets/mainannotated.png')" fluid alt="Responsive image"></b-img>
          </b-col>
        </b-row>
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light">Page when Vertical scrolling on homepage</p>
            <b-img height="400px" width="800px"  :src="require('../assets/scrolling down.png')" fluid alt="Responsive image"></b-img>
          </b-col>
        </b-row>
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light">Carousel interactions</p>
            <b-img height="200px" width="400px"  :src="require('../assets/carousel.png')" fluid alt="Responsive image"></b-img>
          </b-col>
        </b-row>
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light">Footer of homepage</p>
            <b-img height="500px" width="800px"  :src="require('../assets/footer.png')" fluid alt="Responsive image"></b-img>
          </b-col>
        </b-row>
      </b-container> -->



      <p class="m-4 h2 font-weight-bold text-center">Hi-fi for Tablet</p>
      <iframe src="https://drive.google.com/file/d/1C_D_Wez4YXZpQeCyRu6l_jmy-_PiCQOE/preview" width="90%" height="500"></iframe>
      <!-- <b-container class="bv-example-row">
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light">Main Landing Page annotated</p>
            <b-img height="400px" width="700px" :src="require('../assets/landing mobile hi.png')" fluid alt="Responsive image"></b-img>
          </b-col>
        </b-row>
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light">Page when Vertical scrolling on homepage</p>
            <b-img  height="200px" width="600px" :src="require('../assets/tab hi .png')" fluid alt="Responsive image"></b-img>
          </b-col>
        </b-row>
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light">Footer of homepage</p>
            <b-img  height="300px" width="600px" :src="require('../assets/tab footer hi.png')" fluid alt="Responsive image"></b-img>
          </b-col>
        </b-row>
      </b-container> -->


      <p class="m-4 h2 font-weight-bold text-center">Hi-fi for Mobile</p>
      <iframe src="https://drive.google.com/file/d/1jt7eqY9mzJzNxBGF6AUbZJxPqhtvNmZ-/preview" width="90%" height="500"></iframe>
      <!-- <b-container class="bv-example-row">
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light">Main Landing Page annotated</p>
            <b-img height="400px" width="700px" :src="require('../assets/mobile1.png')" fluid alt="Responsive image"></b-img>
          </b-col>
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light">Page when Vertical scrolling on homepage</p>
            <b-img  height="200px" width="600px" :src="require('../assets/mobile2.png')" fluid alt="Responsive image"></b-img>
          </b-col>
        </b-row>
        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light">Footer of homepage</p>
            <b-img  height="300px" width="600px" :src="require('../assets/mobile3.png')" fluid alt="Responsive image"></b-img>
          </b-col>
          <b-col class="text-center m-5">
            <p class="mt-4 h5 font-weight-light">Footer of homepage</p>
            <b-img  height="300px" width="600px" :src="require('../assets/mobile4.png')" fluid alt="Responsive image"></b-img>
          </b-col>
        </b-row>
      </b-container> -->

      <div class="text-center">
        <b-button class="m-5" variant="success" href="#" size="lg" v-scroll-to="'#lo-fi'">LO-FI PROTOTYPE</b-button>
        <b-button class="m-5" variant="success" href="#" size="lg" v-scroll-to="'#redesign'">BACK TO REDESIGN</b-button>
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
