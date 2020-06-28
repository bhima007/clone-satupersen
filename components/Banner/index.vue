<template>
  <v-row no-gutters class="my-12">
    <v-col md="6" sm="6" align-self="center" class="pa-10">
      <p class="banner__quote">
        Platform Tempatmu<br />
        Berkembang Menuju<br />
        #HidupSeutuhnya
      </p>
      <p class="boulder--text">
        Cek artikel-artikel pengembangan diri kami!
      </p>
      <v-btn
        rounded
        class="text-capitalize banner__btn"
        color="primaryyellow"
        x-large
        elevation="10"
        >Baca Artikel <v-icon small class="ml-2">mdi-arrow-right</v-icon></v-btn
      >
    </v-col>
    <v-col md="6" sm="6" class="pa-10">
      <v-img
        src="https://satupersen.net/wp-content/uploads/2020/02/Asset-4-1024x1024.png"
        alt="banner"
        max-height="480"
        max-width="480"
      ></v-img>
    </v-col>
  </v-row>
</template>

<style lang="sass" scoped>
.banner
  &__quote
    font-family: $font-montserrat
    font-size: 40px
    font-weight: 600
    line-height: 1.3em
  &__btn
    font-family: $font-montserrat
    font-weight: 600
    margin-top: 100px
</style>

<style scoped>
@media only screen and (max-width: 425px) {
  .banner__quote{
    font-size: 32px;
  }
}
</style>
