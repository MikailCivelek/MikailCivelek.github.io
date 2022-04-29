<template>
  <v-footer :class="$vuetify.theme.dark ? 'black' : ' white'">
    <v-container>
      <v-divider class="mb-5"></v-divider>
      <v-row class="p-0">
        <v-col class="text--secondary text-center text-md-right d-flex pt-3">
          <div class="d-flex">
            <v-btn
              v-for="(socialm, i) in social"
              :key="`social-${i}`"
              class="d-flex"
              icon
              large
              color="primary"
              :href="socialm.link"
              target="_blank"
            >
              <v-icon>{{ socialm.icon }}</v-icon>
            </v-btn>
          </div>
          <p class="pt-3 ml-3">
            {{ new Date().getFullYear() }} © Mikail Civelek
          </p>
        </v-col>
      </v-row>
    </v-container>
  </v-footer>
</template>

<script>
export default {
  data() {
    return {
      social: [
        {
          platform: 'Facebook',
          link: 'https://www.facebook.com/mikail.civelek.9/',
          icon: 'mdi-facebook',
        },
        {
          platform: 'Twitter',
          link: 'https://twitter.com/',
          icon: 'mdi-twitter',
        },
        {
          platform: 'Instagram',
          link: 'https://www.instagram.com/mikailcivelek/',
          icon: 'mdi-instagram',
        },
        {
          platform: 'Linkedin',
          link: 'https://www.linkedin.com/in/mikail-civelek-be/',
          icon: 'mdi-linkedin',
        },
        {
          platform: 'Github',
          link: 'https://github.com/MikailCivelekPXL',
          icon: 'mdi-github',
        },
      ],
    }
  },
}
</script>

<style>
.site-footer a {
  text-decoration: none;
}
</style>
