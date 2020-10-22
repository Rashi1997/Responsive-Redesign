<template>
  <div>
    <b-jumbotron fluid container-fluid="md" bg-variant="dark" text-variant="white" border-variant="dark" class="full-height">
      <template #header>
        <span class="display-1">Responsive Redesign</span>
      </template>

      <template #lead>
        <span class="h3">Practicing the workflow of redesigning a simple website.</span>
      </template>

      <hr class="my-4" style="color:white;">

      <p>
        This project analyzes the home page of 
        <b-link href="https://torontocupcake.com/#" style="color:white;"><u>Toronto Cupcake</u></b-link> website based on usability and accessibility standards.
        Next, I redesign the homepage of the website by sketching out lo-fi and hi-fi prototypes using Balsamiq Wireframes and Figma respectively. Using these prototypes
        I attempt to recreate the homepage in HTML and CSS (pointing to dummy links) to show how better design can increase the usability of the website.
      </p>
      <b-button variant="primary" href="https://torontocupcake.com/#">ORIGINAL WEBSITE</b-button>
      <b-button variant="success" class="ml-2" href="#" v-scroll-to="'#original'">CURRENT HOMEPAGE & ISSUES</b-button>
    </b-jumbotron>
  </div>
</template>

<script>
export default {
  name: 'Introduction',
  components: {
  }
}
</script>

<style scoped>
  .full-height {
    height: 100%;
    padding-left: 15rem;
    padding-right: 15rem;
    padding-top: 9rem;
    padding-bottom: 15rem;
    margin-bottom: 0;
  }
  hr {
    border:0.01rem solid white;
  }
</style>
