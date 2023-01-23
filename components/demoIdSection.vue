<template>
  <div>
    <v-container class="main-section3" fluid pa-0>
      <v-img
        class="main-section3bg"
        :src="require(`@/assets/media/demoIdSection.webp`)"
      >
        <v-container>
          <v-row no-gutters>
            <v-col cols="12" sm="6" class="content">
              <v-card-title class="white--text pt-5">
                <div>
                  <h1>GET YOUR DEMO ID</h1>
                </div>
                <v-text class="">
                  <div class="main-content">
                    Are you an avid trader? Are you starting out? Worry not,
                    we’ve made it easy! Click here to get a Demo ID and take a
                    virtual tour.
                  </div>
                </v-text>
              </v-card-title>
              <v-card class="pa-4 card mt-8" elevation="0" title>
                <v-hover v-slot="{ hover }">
                  <v-btn
                    class="idbtn rounded-0 pt-7 pb-7 mb-5 mb-md-0"
                    outlined
                    :style="{
                      'background-color': hover ? '#07083A' : 'transparent',
                    }"
                  >
                    ID: 90008
                  </v-btn>
                </v-hover>
                <v-hover v-slot="{ hover }">
                  <v-btn
                    class="rounded-0 pt-7 pb-7 mb-5 mb-md-0"
                    outlined
                    :style="{
                      'background-color': hover ? '#07083A' : 'transparent',
                    }"
                  >
                    Pass: demo12345
                  </v-btn>
                </v-hover>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6">
              <v-img
                :src="require(`@/assets/media/Design.webp`)"
                max-width="350px"
                class="main-section3img ml-16"
              >
              </v-img>
            </v-col>
          </v-row>
        </v-container>
      </v-img>
    </v-container>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
h1 {
  font-family: "Bebas Neue", cursive;
}
.banner-img {
  height: 100vh;
  background: transparent;
  color: aliceblue;
}
.card {
  background-color: transparent;
  color: white;
}
.num {
  max-width: 100%;
  max-height: 100%;
}

@media screen and (min-width: 150px) and (max-width: 599px) {
  .main-section3img {
    display: none;
  }
}

@media only screen and (min-width: 1024px) {
  .content {
    padding: 30px;
    z-index: 2;
  }
  .tradebg-img {
    z-index: 1;
  }
  .bg3 {
    z-index: 1;
  }
  .hand-img {
    z-index: 2;
  }
  .main-section3 {
    position: relative;
    z-index: 1111;
  }
  .main-section3bg {
    position: initial;
  }
  .main-section3img {
    position: absolute;
    z-index: 1;
    bottom: -33px;
  }
  .v-card__title {
    word-break: break-word;
    line-height: inherit;
  }
}
.main-content {
  font-family: "Montserrat", sans-serif;
  word-break: break-word;
}
@media only screen and (min-width: 280px) {
  .v-card__title {
    word-break: break-word;
    line-height: inherit;
  }
}
</style>
