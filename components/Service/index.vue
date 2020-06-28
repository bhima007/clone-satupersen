<template>
  <div
    id="service"
    class="d-flex flex-column align-center justify-center alabaster py-50 service"
  >
    <span class="primaryyellow--text my-title">Produk &amp; Layanan Kami</span>
    <v-row no-gutters class="d-flex flex-wrap mt-10">
      <v-col cols="3" v-for="(item, i) in items" :key="i">
        <v-card
          flat
          width="239"
          tile
          class="d-flex flex-column align-center pa-1 text-center alabaster service__card"
        >
          <img height="146" :src="item.img" />
          <a
            :href="item.link"
            v-text="item.title"
            class="mineshaft--text mt-6 mb-2"
          ></a>
          <p v-text="item.description" class="dovegrey--text px-1"></p>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          img:
            'https://satupersen.net/wp-content/uploads/2020/02/Mentoring.jpg',
          title: 'Mentoring',
          link: '#service',
          description:
            'Konsultasi 1 on 1 secara online atau offline dengan Mentor dari Satu Persen.',
        },
        {
          img:
            'https://satupersen.net/wp-content/uploads/2020/02/Konseling.jpg',
          title: 'Konseling',
          link: '#service',
          description:
            'Terapi dan Konseling 1 on 1 secara online atau offline dengan Psikolog dari Satu Persen.',
        },
        {
          img: 'https://satupersen.net/wp-content/uploads/2020/02/Event.jpg',
          title: 'Events',
          link: '#service',
          description:
            'Kelas, workshop, atau seminar interaktif yang membahas topik-topik menarik tentang kehidupan.',
        },
        {
          img: 'https://satupersen.net/wp-content/uploads/2020/02/Webinar.jpg',
          title: 'Online Class & Webinar',
          link: '#service',
          description:
            'Kelas online untuk belajar tentang hal-hal penting dalam hidup.',
        },
      ],
    }
  },
}
</script>

<style lang="sass" scoped>
.service
  &__card
    a
      font-size: 20px
      font-weight: 600
    a:hover
      color: $color-primary-yellow !important
      text-decoration: none
    p
      font-size: 15px
      font-weight: 600
      line-height: 24px
</style>
