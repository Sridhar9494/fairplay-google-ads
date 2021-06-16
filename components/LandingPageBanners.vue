<template>
  <div>
    <!-- desktop view -->
    <div class="hidden-sm-and-downqqq">
      <v-row v-for="(slide, i) in desktopBanners" :key="i" no-gutters>
        <v-col cols="12">
          <div class="d-flex align-center">
            <v-img
              :src="require(`assets/images/banner/${slide.image}.jpg`)"
              aspect-ratio="2"
            ></v-img>
          </div>
        </v-col>
      </v-row>
    </div>

    <!-- <div class="hidden-md-and-up">
      <v-row v-for="(slide, i) in mobileBanners" :key="i" no-gutters>
        <v-col cols="12">
          <div class="d-flex align-center lorem">
            <v-img
              :src="require(`assets/images/banner/${slide.image}.jpg`)"
              aspect-ratio="2"
            ></v-img>
          </div>
        </v-col>
      </v-row>
    </div> -->
  </div>
</template>

<script>
export default {
  data() {
    return {
      desktopBanners: [
        {
          image: 'desktop_banner_1',
        },
        {
          image: 'desktop_banner_2',
        },
      ],
      mobileBanners: [
        {
          image: 'mobile_banner_1',
        },
        {
          image: 'mobile_banner_2',
        },
      ],
    }
  },
}
</script>

<style lang="scss" scoped></style>
