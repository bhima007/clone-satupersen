<template>
  <div id="testimoni" class="d-flex flex-column align-center py-50">
    <p class="primaryyellow--text my-title">
      Testimoni
    </p>
    <div class="d-flex flex-wrap align-center justify-center">
      <!-- <v-carousel
        cycle
        height="400"
        hide-delimiter-background
        show-arrows-on-hover
      >
        <v-carousel-item v-for="(item, i) in items" :key="i">
          <v-sheet height="100%">
            <v-row class="fill-height" align="center" justify="center"> -->
      <v-card
        v-for="(item, i) in items"
        :key="i"
        flat
        max-width="474"
        class="d-flex flex-column align-center text-center mt-5 mx-4"
      >
        <div>
          <v-avatar size="100" class="elevation-18">
            <img :src="item.img" alt="avatar" />
          </v-avatar>
        </div>
        <p
          v-text="item.evaluate"
          class="testimoni__card__evaluate dovegrey--text mt-8"
        ></p>
        <span
          v-text="item.info.name"
          class="testimoni__card__info mineshaft--text pb-1"
        ></span>
        <span
          v-text="item.info.job"
          class="testimoni__card__info__job dovegrey--text pb-1"
        ></span>
      </v-card>
      <!-- </v-row>
          </v-sheet>
        </v-carousel-item>
      </v-carousel> -->
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          img:
            'https://satupersen.net/wp-content/uploads/2020/02/Foto-Fakkar-Mentee.png',
          evaluate:
            '"Berdampak banget, karena pelajaran tentang bagaimana cara dalam menghadapi kehidupan dengan baik ada di sini. Recommended banget, semoga visi dari Satu Persen bisa terlaksana & berdampak lebih besar lagi"',
          info: {
            name: 'Fakkar',
            job: 'Mentee',
          },
        },
        {
          img:
            'https://satupersen.net/wp-content/uploads/2020/02/Foto-Tsabitah-Mentee.png',
          evaluate:
            '"Lebih ingat untuk mencintai diri sendiri. Fokus ke solusi permasalahan, terus sadar kalo setiap manusia wajar kalo insecure tapi jangan lupa kita punya kelebihan dan keunikan tersendiri sebagai manusia"',
          info: {
            name: 'Tsabitah',
            job: 'Mentee',
          },
        },
      ],
    }
  },
}
</script>

<style lang="sass" scoped>
.testimoni
  &__card
    &__evaluate
      font-size: 18px
      font-weight: 600
      font-style: italic
      line-height: 29px
    &__info
      font-size: 20px
      font-weight: 600
      &__job
        font-size: 15px
        font-weight: 600
</style>
