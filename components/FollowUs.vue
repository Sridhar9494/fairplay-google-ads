<template>
  <div class="mb-10">
    <div>
      <div
        class="
          text-uppercase
          mb-4
          text-center
          primary--text
          display-1
          font-weight-bold
        "
      >
        Follow US
      </div>
    </div>
    <div class="text-center mb-10">
      <v-btn
        v-for="item in socialMedia"
        :key="item.icon"
        class="ma-1 py-4"
        target="_blank"
        rel="noreferrer"
        aria-label="fairplay_social_media"
        :href="item.link"
        tile
        height="60"
        min-width="60"
      >
        <v-icon>{{ item.icon }}</v-icon>
      </v-btn>
    </div>
    <div class="text-center footer-section">
      <v-btn class="mx-2" fab dark large disabled
        ><span class="white--text headline"> 18+</span>
      </v-btn>

      <div class="gc-image white">
        <v-img
          contain
          src="https://fairplay-image.fairplay.club/gc.png"
          aspect-ratio="2"
          height="60"
          width="100"
          class="text-center white"
          alt="gaming curacao logo"
        ></v-img>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      socialMedia: [
        {
          icon: 'fab fa-facebook-f',
          link: 'https://www.facebook.com/FairPlay-103941624783096/',
        },
        {
          icon: 'fab fa-twitter',
          link: 'https://twitter.com/FairPlay_India',
        },
        {
          icon: 'fab fa-instagram',
          link: 'https://instagram.com/fairplay_india',
        },
        {
          icon: 'fab fa-telegram-plane',
          link: 'https://t.me/officialfairplay',
        },
        {
          icon: 'fab fa-youtube',
          link: 'https://www.youtube.com/channel/UCDgi_kPO-5gCT5YoKj2TSsA?view_as=subscriber',
        },
        {
          icon: 'fab fa-linkedin-in',
          link: 'https://www.linkedin.com/company/fairplayclub/',
        },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.social-media a {
  margin-left: -3px;
}

.footer-section {
  position: relative;
  .gc-image {
    position: absolute;
    right: 0;
    top: 3px;
  }
}
</style>
