<template>
  <div>
    <v-container fluid class="landing">
      <v-img :src="require('@/assets/media/mainBanner.webp')">
        <v-container>
          <v-row>
            <v-card-title class="white--text pt-10">
              <!-- <h1>Fairplay Market</h1> -->
              <v-img
                :src="require('@/assets/media/logo.webp')"
                max-height="205"
                max-width="250"
                class="logo"
              >
              </v-img>
            </v-card-title>
          </v-row>
          <v-row>
            <v-col cols="12 " sm="6" xl="12" class="content">
              <v-row class="mt-2">
                <v-col
                  v-for="title in Data"
                  :key="title.id"
                  cols="12"
                  sm="12"
                  class="mb-3"
                >
                  <div>
                    <v-card class="card d-flex" elevation="0" title>
                      <v-card-title>
                        <div class="d-flex">
                          <div>
                            <v-img
                              :src="require(`../assets/media/Line.webp`)"
                              class="mr-5"
                            >
                            </v-img>
                          </div>
                          <div>
                            <v-img
                              :src="require(`../assets/media/` + title.icon)"
                              class="num mr-5"
                            >
                            </v-img>
                          </div>
                          <div class="main-content">
                            {{ title.Title }}
                          </div>
                        </div>
                      </v-card-title>
                    </v-card>
                  </div>
                </v-col>
              </v-row>
            </v-col>
            <v-col cols="12" sm="6" xl="12" class="phone-img">
              <v-card-title>
                <v-img
                  :src="require(`../assets/media/Vector-Smart-ObjectDWDW.webp`)"
                >
                </v-img>
              </v-card-title>
            </v-col>
          </v-row>
        </v-container>
      </v-img>
    </v-container>
  </div>
</template>

<script>
import { computed } from "vue";

export default {
  data() {
    return {
      Data: [
        {
          id: 1,
          Title: "Daily Withdrawal",
          icon: "01.webp",
          description:
            "Quick and easy access to your money any time on (FairPlay Share Market?). Avail daily withdrawals and trade faster and better!",
        },
        {
          id: 2,
          Title: "Low Brokerage",
          icon: "02.webp",
          description:
            "High market brokerage eating away at your profits? Not anymore! With (FP Share Market?)’s lowest (?) brokerage, your money is all yours!",
        },
        {
          id: 3,
          Title: "No DMAT and KYC required",
          icon: "03.webp",
          description:
            "Do away with lengthy account creation and verification troubles with FPSM’s hassle free trading. All you need is ______ to get started and get trading.",
        },
        {
          id: 4,
          Title: "MCX/ NSE/ COMEX markets available",
          icon: "04.webp",
          description:
            "FPSM is your one stop shop for all your trading needs. Find all the popular markets under one roof and gain big profits.",
        },
      ],
    };
  },
  computed: {
    width() {
      switch (this.$vuetify.breakpoint.name) {
        case "xs":
          return 250;
      }
    },
  },
};
</script>

<style scoped>
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
.main-content {
  font-family: "Montserrat", sans-serif;
  word-break: break-word;
}
@media only screen and (min-width: 1024px) {
  .content {
    padding: 30px;
    z-index: 2;
  }

  .tradebg-img,
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
  /* .main-section1 {
    /* position: relative;
    z-index: 1111; 
  } */
  .main-section1bg {
    position: initial;
  }
  .main-section1img {
    position: absolute;
    z-index: 1;
    right: 0;
    bottom: -33px;
    width: 470px;
  }
  .v-card__title {
    word-break: break-word;
    line-height: inherit;
  }
  h1 {
    font-family: "Bebas Neue", cursive;
  }
  .main-content {
    font-family: "Montserrat", sans-serif;
  }
}
.main-content {
  font-family: "Montserrat", sans-serif;
  word-break: break-word;
}
@media only screen and (min-width: 280px) {
  h1 {
    font-family: "Bebas Neue", cursive;
  }
  .logo {
    max-width: 400px;
  }
  .main-content {
    font-family: "Montserrat", sans-serif;
  }
  .main-content {
    font-family: "Montserrat", sans-serif;
    word-break: break-word;
  }
}
.landing {
  background-image: url("../assets/media/mainBanner.webp");
}
</style>
