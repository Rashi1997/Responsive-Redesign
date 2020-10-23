<template>
  <div>
    <b-jumbotron fluid container-fluid="md" bg-variant="white" border-variant="dark" class="full-height">
      <template #header>Hi-Fi Prototype</template>

      <template #lead>
        The Hi-fi prototypes were created and annotated using Figma, with all the hover state and scrolling interactions.
      </template>

      
      <b-container class="bv-example-row">
        <b-row align-v="center">
          <b-col class="text-center m-5">

            <p class="m-4 h2 font-weight-bold text-center">Hi-fi for Desktop</p>
            <iframe class src="https://drive.google.com/file/d/1kuZ8-MiXc-5A4zs9QrEQ6ZwTIucVeXoU/preview" width="90%" height="500"></iframe>

          </b-col>
        </b-row>

        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="m-4 h2 font-weight-bold text-center">Hi-fi for Tablet</p>
            <iframe src="https://drive.google.com/file/d/1Jxc95Epv650bJgGSZz938PS9rH_PZ9N9/preview" width="90%" height="500"></iframe>
          </b-col>
        </b-row>

        <b-row align-v="center">
          <b-col class="text-center m-5">
            <p class="m-4 h2 font-weight-bold text-center">Hi-fi for Mobile</p>
            <iframe src="https://drive.google.com/file/d/1vpnt00IqbEKOef2J35N76FMr985uNXiz/preview" width="90%" height="500"></iframe>
          </b-col>
        </b-row>
      </b-container>



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
        <b-button class="m-5" variant="success" href="#" size="lg" v-scroll-to="'#visual'">VISUAL STYLE GUIDE</b-button>
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
