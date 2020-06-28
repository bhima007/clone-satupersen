<template>
  <v-app dark>
    <App-Header></App-Header>

    <v-divider></v-divider>

    <v-main>
      <div class="my-container">
        <nuxt />
      </div>
    </v-main>

    <App-Footer></App-Footer>

    <Social-Media></Social-Media>

    <!-- <v-speed-dial
      v-model="fab"
      bottom
      right
      fixed
      transition="slide-y-reverse-transition"
    >
      <template v-slot:activator>
        <v-btn v-model="fab" fab class="primaryyellow">
          <v-icon>mdi-share</v-icon>
        </v-btn>
      </template>
      <v-btn fab dark class="facebook" small>
        <v-icon>mdi-facebook</v-icon>
      </v-btn>
    </v-speed-dial> -->
  </v-app>
</template>

<script>
import AppHeader from '@/components/Header/index'
import AppFooter from '@/components/Footer/index'
import SocialMedia from '@/components/SocialMedia/index'

export default {
  components: {
    AppHeader,
    AppFooter,
    SocialMedia,
  },
  data() {
    return {
      fab: false,
    }
  },
}
</script>

<style lang="sass">
html
  scroll-behavior: smooth
.my-container
  max-width: 1029px
  margin: 0 auto
.my-title
  font-size: 28px
  font-weight: 600
  line-height: 1
.py-50
  padding: 50px 0
</style>

<style>
@media only screen and (max-width: 960px) {
  .my-title {
    font-size: 26px;
  }
}
</style>
