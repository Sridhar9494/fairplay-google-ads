<template>
  <div>
    <div class="my-4">
      <v-img
        src="https://fairplay-image.fairplay.club/logo.png"
        max-height="70"
        contain
        class="darken-4"
      ></v-img>
    </div>
    <landing-page-banners />
    <v-container>
      <features />
      <follow-us />
    </v-container>
  </div>
</template>

<script>
/*eslint-disable*/
import FollowUs from '@/components/FollowUs'
import Features from '@/components/Features'
import LandingPageBanners from '@/components/LandingPageBanners'

export default {
  components: {
    Features,
    LandingPageBanners,
    FollowUs,
  },
  data() {
    return {}
  },
}
</script>

<style lang="scss" scoped>
.width-80 {
  width: 80%;
}
</style>
