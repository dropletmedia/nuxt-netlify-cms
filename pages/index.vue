<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
      xs12
      sm8
      md6
    >
      <div class="text-center">
        
      </div>
      <v-card>
        <v-card-title class="headline">
          Vuetify + Nuxt.js + Vuex + Netlify CMS template
        </v-card-title>
        <v-card-text>
          <p>See this doc for setup </p>
          <p><a href="https://www.netlifycms.org/docs/nuxt/">https://www.netlifycms.org/docs/nuxt/</a></p>
        </v-card-text>
         
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/blog"
          >
            Blog
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>


export default {
  components: {
   
  },
  head() {
    return {
      script: [{ src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }],
    };
  },
}
</script>
