<template>
  <div>
    <v-row no-gutters class="pb-16">
      <v-col v-for="item in features" :key="item.name" cols="6" sm="3" md="3">
        <div class="text-center">
          <v-img
            :src="require(`@/assets/images/features/${item.image}.png`)"
            class="mx-auto"
            width="100"
          ></v-img>
          <div class="text-capitalize font-weight-bold">{{ item.name }}</div>
        </div>
      </v-col>
    </v-row>

    <v-row no-gutters class="pb-16 text-center">
      <v-col cols="12" sm="12" md="12">
        <v-btn
          href="https://fairplay.club/"
          target="_blank"
          height="64"
          class="px-16"
          color="primary"
        >
          <span class="display-1">PLAY NOW</span>
        </v-btn>
      </v-col>
    </v-row>

    <v-row no-gutters justify="center" class="pb-16">
      <v-col
        v-for="item in featuresBtns"
        :key="item.name"
        cols="12"
        sm="6"
        md="6"
      >
        <div class="pa-1">
          <v-btn class="align-self-center text-capitalize" tile block>
            <span class="font-weight-bold">{{ item.name }}</span>
          </v-btn>
        </div>
      </v-col>
    </v-row>

    <v-row no-gutters class="pb-16">
      <v-col cols="12" sm="12" md="12">
        <div class="text-capitalize text-justify">
          Get the most profitable odds in the market on India' s favourite
          exchange- FairPlay! We stream all major Cricket, Football and Tennis
          matches live for our Club members to watch while playing alongside!
          Not just that, we also offer many fancy market and advance market
          options! FairPlay has covered T20 cricket leagues like IPL & PSL, the
          Big Bash League, Cricket World Cup and many more. Not just that, the
          likes of EPL, Champions League, La Liga, Euro Cup and also French
          Open, Australian Open, US Open, Wimbledon and so much more!
          <br />
          <br />
          Live casino games include several variations of Roulette, BlackJack,
          Baccarat, Poker and Show games. Indian card games like Teen Patti,
          Andar Bahar, Poker, 7Up 7Down, Andar Bahar and so many more are also
          conducted by live dealers on FairPlay.
          <br />
          <br />
          Find tutorials for all games on the website as well as on the social
          media. Reach out to our Client Services team for further assistance.
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      features: [
        {
          name: 'instant withdrawals & deposits',
          image: 'feature01',
        },
        {
          name: 'live stream of events',
          image: 'feature02',
        },
        {
          name: '24/7 customer service',
          image: 'feature03',
        },
        {
          name: 'multiple payment options',
          image: 'feature04',
        },
      ],
      featuresBtns: [
        {
          name: 'Why fairplay?',
        },
        {
          name: 'Responsible Gaming',
        },
        {
          name: 'Promotions',
        },
        {
          name: 'privacy policy',
        },
        {
          name: 'Terms & conditions',
        },
      ],
    }
  },
}
</script>

<style></style>
