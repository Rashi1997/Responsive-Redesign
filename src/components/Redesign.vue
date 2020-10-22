<template>
  <div>
    <b-jumbotron fluid container-fluid="md" bg-variant="light" border-variant="dark" class="full-height">
      <template #header>
        Redesign
      </template>

      <template #lead>
        <p>Next I sketched Low-fidelity and High-fidelity prototypes for desktop, tablet and mobile to show how the focus of the website can be shifted
        to the products on the homepage and the COVID update can be shifted as an alert instead of occupying the whole homepage.</p>
        <p>
           I also redesigned the menu bar to have direct links to what users want to find on the website. The original website had everything hidden inside the
          menu and it is difficult for the user to go and look for information in sliding menu on the ecommerce website. I specifically put the flavors, stores and cart in the upper
          menu bar. The second menu bar is for the other specialities like Halloween, Occasions and Coorporate events.
        </p>
        <p>
          On an ecommerce website it is usually easier to have a search field to directly find what you are looking for, the current design does not support that.
          So I included a search field on the top navigation bar. 
        </p>
      </template>
      <div class="text-center">
        <b-button class="m-5" variant="success" href="#" size="lg" v-scroll-to="'#lo-fi'">LO-FI PROTOTYPE</b-button>
        <b-button class="m-5" variant="success" href="#" size="lg" v-scroll-to="'#redesign'">HI-FI PROTOTYPE</b-button>
      </div>

    </b-jumbotron>
  </div>
</template>

<script>

export default {
  name: 'Redesign',
  components: {
  }
}
</script>

<style scoped>
  .full-height {
    height: 100vh;
    padding-bottom: 0;
    margin-bottom: 0;
    border: 0!important;
  }
</style>
