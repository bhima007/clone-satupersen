<template>
  <div class="d-none d-sm-flex justify-center social-media">
    <v-btn
      v-for="(item, i) in items"
      :key="i"
      fab
      dark
      class="mx-1 button"
      :class="item.media"
      small
    >
      <v-icon>mdi-{{ item.media }}</v-icon>
    </v-btn>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { media: 'facebook' },
        { media: 'twitter' },
        { media: 'youtube' },
        { media: 'linkedin' },
        { media: 'instagram' },
      ],
    }
  },
}
</script>

<style lang="sass" scoped>
.social-media
  width: 100%
  position: fixed !important
  bottom: 5px
  .button
    opacity: 0.4
  .button:hover
    opacity: 1
</style>
