<template>
  <div>
    <b-jumbotron fluid container-fluid="md" bg-variant="white" border-variant="dark" class="full-height">
      <template #header>Current Homepage & Issues</template>

      <template #lead>
        I choose the homepage of this website because because the current design does not do justice to the cupcakes
        and is not appealing to the users. The homepage also seems like a fake ecommerce site and makes users question the authenticity of the website.
        I have listed the issues with the current design (on left) below.
      </template>
      <b-container class="bv-example-row">
        <b-row  class="mb-5" align-v="center">
          <b-col>
            <b-img :src="require('../assets/original_mobile.png')" fluid alt="Responsive image"></b-img>
          </b-col>
          <b-col>
            <div>
              <b-table striped hover :items="items">
                <template #cell(guidline)="data">
                  <!-- `data.value` is the value after formatted by the Formatter -->
                  <span class="font-weight-bold">{{ data.value }}</span>
                </template>
              </b-table>
            </div>
          </b-col>
        </b-row>
        <hr>
        <b-row  class="mt-5 mb-5" align-v="center">
          <b-col>
            <b-img :src="require('../assets/menu issue.png')" fluid alt="Responsive image"></b-img>
            <p class="m-4 h5 font-weight-light text-center">Hidden menu bar and sticky dropdown on cupcakes</p>
          </b-col>
          <b-col>
            <b-img :src="require('../assets/screen reader.png')" fluid alt="Responsive image"></b-img>
            <p class="m-4 h5 font-weight-light text-center">Hidden Text below the footer which interferes with the screen reader</p>
          </b-col>
        </b-row>
        <b-row align-v="center">
          <b-col>
            <p class="m-4 h2 font-weight-bold text-center">Accessibility Issues</p>
          </b-col>
        </b-row>
        <b-row align-v="center">
          <b-col>
            <div>
              <b-table striped hover :items="issues">
                <template #cell(guidline)="data">
                  <!-- `data.value` is the value after formatted by the Formatter -->
                  <span class="font-weight-bold">{{ data.value }}</span>
                </template>
              </b-table>
            </div>
          </b-col>
        </b-row>
      </b-container>
      <div class="text-center">
        <b-button class="m-5" variant="success" href="#" size="lg" v-scroll-to="'#redesign'">REDESIGN</b-button>
      </div>
    
    </b-jumbotron>
  </div>
</template>

<script>

export default {
  data() {
    return {
      items: [
        { guidline: 'Intuitive Design', Issue: 'The homepage is mostly filled with the COVID update and the boxes of cupcakes. The Menu is far away from the rest of the site at top left and is almost impossible to find. The footer is just a plain line of links with no contact information is almost non-existent. It doesn’t get much better as you get deeper into the site—if you can get there.' },
        { guidline: 'Ease of Learning', Issue: 'There are no social media links on the site and the site disconnected from digital marketing. ' },
        { guidline: 'Efficiency of Use', Issue: 'An ecommerce website should have the products displayed on the homepage for the ease of user, which is inside the hidden menu and cupcakes dropdown here.' },
        { guidline: 'Memorability', Issue: 'The footer is just a plain line of links with no contact information is almost non-existent. Comic Sans is used as the main font and there is no font hierarchy, which makes it hard to remember the website.' },
        { guidline: 'Error Frequency and Satisfication', Issue: 'We always seem to get stuck in the cupcakes submenu dropdown in the collapsible side menu bar.' },
        { guidline: 'Subjective Satisfaction', Issue: 'The many logos at the top are an overkill. The site is not aesthetic at all and does not look as pleasing as a cupcake website should be. ' }
      ],
      issues: [
        { guidline: 'Intuitive Design', Issue: 'The homepage is mostly filled with the COVID update and the boxes of cupcakes. The Menu is far away from the rest of the site at top left and is almost impossible to find. The footer is just a plain line of links with no contact information is almost non-existent. It doesn’t get much better as you get deeper into the site—if you can get there.' },
        { guidline: 'Ease of Learning', Issue: 'There are no social media links on the site and the site disconnected from digital marketing. ' },
        { guidline: 'Efficiency of Use', Issue: 'An ecommerce website should have the products displayed on the homepage for the ease of user, which is inside the hidden menu and cupcakes dropdown here.' },
        { guidline: 'Memorability', Issue: 'The footer is just a plain line of links with no contact information is almost non-existent. Comic Sans is used as the main font and there is no font hierarchy, which makes it hard to remember the website.' },
        { guidline: 'Error Frequency and Satisfication', Issue: 'We always seem to get stuck in the cupcakes submenu dropdown in the collapsible side menu bar.' },
        { guidline: 'Subjective Satisfaction', Issue: 'The many logos at the top are an overkill. The site is not aesthetic at all and does not look as pleasing as a cupcake website should be. ' }
      ]
    }
  },
  name: 'OriginalWebsite',
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
