<template>
  <div>
    <App-Banner></App-Banner>
    <App-About></App-About>
    <App-Testimoni></App-Testimoni>
    <App-Service></App-Service>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'
import AppBanner from '@/components/Banner/index'
import AppAbout from '@/components/About/index'
import AppTestimoni from '@/components/Testimoni/index'
import AppService from '@/components/Service/index'

export default {
  components: {
    Logo,
    VuetifyLogo,
    AppBanner,
    AppAbout,
    AppTestimoni,
    AppService,
  },
}
</script>
