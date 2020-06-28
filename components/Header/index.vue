<template>
  <div>
    <v-container>
      <div class="d-flex align-center">
        <img
          src="https://satupersen.net/wp-content/uploads/2020/02/SatuPersen-Logo-With-Word.png"
          class="header__logo"
        />
        <v-spacer />
        <div class="d-none d-md-flex header__menu mineshaft--text">
          <a href="#about">Tentang</a>
          <a href="#testimoni">Testimoni</a>
          <a href="#service">Layanan</a>
          <a href="#blog">Blog</a>
          <a href="#event">Event</a>
          <a href="#test">Online Test</a>
        </div>
        <v-btn
          class="d-flex d-md-none"
          outlined
          tile
          icon
          @click.stop="rightDrawer = !rightDrawer"
        >
          <v-icon>mdi-menu</v-icon>
        </v-btn>
      </div>

      <v-navigation-drawer v-model="rightDrawer" :right="right" temporary fixed>
        <v-list>
          <v-list-item @click.native="right = !right">
            <v-list-item-action>
              <v-icon light>
                mdi-repeat
              </v-icon>
            </v-list-item-action>
            <v-list-item-title>Switch drawer (click me)</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
    }
  },
}
</script>

<style lang="sass" scoped>
.header
  &__logo
    height: 50px
  &__menu
    a
      color: inherit
      text-decoration: none
      margin: 0 10px
    a:hover
      color: $color-primary-yellow
</style>

<style scoped>
@media only screen and (max-width: 960px) {
  .header__logo {
    height: 40px;
  }
}
</style>
