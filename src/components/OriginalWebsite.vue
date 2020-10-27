<template>
  <div>
    <b-jumbotron fluid container-fluid="md" bg-variant="white" border-variant="dark" class="full-height">
      <template #header>Current Homepage & Issues</template>

      <template #lead>
        I choose the homepage of this website because the current design does not do justice to the cupcakes
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


        <b-row  class="mt-5 mb-5" align-v="center">
          <b-col class="text-center">
            <b-img width="200px" height="300px" :src="require('../assets/report1.png')" fluid alt="Responsive image"></b-img>
            <p class="m-4 h5 font-weight-light text-center">Wave Accessibility Report</p>
          </b-col>
          <b-col class="text-center">
            <b-img width="200px" height="300px" :src="require('../assets/report2.png')" fluid alt="Responsive image"></b-img>
            <p class="m-4 h5 font-weight-light text-center">Wave Accessibility Report: many contrast errors and three alerts.</p>
          </b-col>
        </b-row>

        <b-row  class="mt-5 mb-5" align-v="center">
          <b-col class="text-center">
            <b-img width="500px" height="500px" :src="require('../assets/s1.png')" fluid alt="Responsive image"></b-img>
            <p class="m-4 h5 font-weight-light text-center">The menu has an alert for not being accessible, <b>the corporate/event logo cupcakes - Click for details</b> link has a suspicious link text alert. The text below the COVID 19 text has an alert for being justified. See table for more details</p>
          </b-col>
          <b-col class="text-center">
            <b-img width="600px" height="700px" :src="require('../assets/s2.png')" fluid alt="Responsive image"></b-img>
            <p class="m-4 h5 font-weight-light text-center">The h4 header occurs before the h1 header and the website has no hierarchy for font size.</p>
          </b-col>
        </b-row>

        <b-row  class="mt-5 mb-5" align-v="center">
          <b-col class="text-center">
            <b-img width="500px" height="500px" :src="require('../assets/s3.png')" fluid alt="Responsive image"></b-img>
            <p class="m-4 h5 font-weight-light text-center">At the end of the website there is a lot of white text which has low contrast errors.</p>
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
        { guidline: 'Efficiency of Use', Issue: 'The occasions based cupcakes are missing from the direct view of the user. An ecommerce website should have the products displayed on the homepage for the ease of user, which is inside the hidden menu and cupcakes dropdown here.' },
        { guidline: 'Memorability', Issue: 'The footer is just a plain line of links with no contact information is almost non-existent. Comic Sans is used as the main font and there is no font hierarchy, which makes it hard to remember the website.' },
        { guidline: 'Error Frequency and Satisfication', Issue: 'We always seem to get stuck in the cupcakes submenu dropdown in the collapsible side menu bar.' },
        { guidline: 'Subjective Satisfaction', Issue: 'The many logos at the top are an overkill. The site is not aesthetic at all and does not look as pleasing as a cupcake website should be. ' }
      ],
      issues: [
        { Issue: 'Keyboard accessibility', Comment: 'The menu is not accessible with tab. Also when tabbing through the website, the image of the cupcake boxes is also a link which has poor visible focus and the user could seem lost. The major contents of the website are in the menu which is not accessible to someone with physical limitations who do not use a mouse and rely on other mechanisms such as the keyboard, voice control,  and other pointing devices to navigate and interact with the Web. So the website is basically useless to them as they cannot shop around for cupcakes.'},
        { Issue: 'Screen reader', Comment: 'The screen reader skips the menu.'},
        { Issue: 'Contrast Errors', Comment: 'The text below the footer is white in color and suffers from very low contrast between text and background colors as sdequate contrast of text is necessary for all users, especially users with low vision.'},
        { Issue: 'Suspicious link text', Comment: 'Link text for corporate/event logo cupcakes - Click for details in header contains extraneous text or may not make sense out of context.'},
        { Issue: 'Justified text', Comment: 'Fully justified text is present below the COVID 19 text and these large blocks of justified text can negatively impact readability due to varying word/letter spacing and rivers of white that flow through the text.'}
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
