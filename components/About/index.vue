<template>
  <div id="about" class="alabaster pa-3">
    <div class="d-flex flex-column align-center text-center py-50">
      <iframe
        class="about__youtube mb-10"
        src="https://www.youtube.com/embed/EXfY_JLbyS4?feature=oembed&playlist=EXfY_JLbyS4&wmode=opaque&loop=1&controls=0&mute=0&rel=0&modestbranding=0"
      ></iframe>

      <p class="primaryyellow--text my-title">
        Dimulai Dari Channel Youtube Edukasi
      </p>

      <p class="boulder--text about__description">
        Satu Persen percaya bahwa setiap orang bisa berkembang dan berdaya.
        Sejak awal tahun 2019, Satu Persen telah berkontribusi besar dalam
        pemberian konten edukasi kesehatan mental dan pengembangan diri.
        <em>Channel Youtube</em> Satu Persen saat ini telah mencapai lebih dari
        500 ribu <em>subscribers</em>. Layanan Satu Persen, mulai dari
        <em>mentoring</em>, <em>konseling</em>, kelas dan lainya telah membantu
        ribuan orang untuk bangkit dan menjadi berdaya.
      </p>
    </div>
  </div>
</template>

<style lang="sass" scoped>
.about
  &__youtube
    border: none
    width: 478px
    height: 269px
  &__description
    font-size: 20px
    padding: 0 30px
</style>

<style scoped>
@media only screen and (max-width: 960px) {
  .about__youtube {
    width: 338px;
    height: 190px;
  }
  .about__description {
    font-size: 14px;
  }
}
</style>
