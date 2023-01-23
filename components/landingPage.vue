<template>
  <div>
    <v-container fluid pa-0>
      <v-img :src="require('@/assets/media/mainBanner.webp')">
        <v-container>
          <v-row>
            <v-card-title class="white--text mt-2">
              <!-- <h1>Fairplay Market</h1> -->
              <v-img
                :src="require('@/assets/media/logo.webp')"
                max-width="230"
                class="logo"
              >
              </v-img>
            </v-card-title>
          </v-row>
          <v-row>
            <v-col cols="12 " sm="6" xl="12" class="content">
              <v-row>
                <v-col
                  v-for="title in Data"
                  :key="title.id"
                  cols="12"
                  sm="12"
                  class="pa-md-4 pa-0"
                >
                  <div>
                    <v-card class="card d-flex" elevation="0" title>
                      <v-card-title>
                        <div class="d-flex">
                          <v-img
                            :src="require(`../assets/media/Line.webp`)"
                            class="mr-2 mt-1"
                            max-height="25"
                          >
                          </v-img>
                          <v-img
                            :src="require(`../assets/media/` + title.icon)"
                            class="num mr-3 mt-1"
                            max-height="25"
                            max-width="22"
                          >
                          </v-img>

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
              <v-img
                class="mx-img"
                max-width="400"
                :src="require(`../assets/media/Vector-Smart-ObjectDWDW.webp`)"
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
};
</script>

<style scoped>
.main-content {
  font-family: "Montserrat", sans-serif;
  word-break: break-word;
}
.banner-img {
  height: 100vh;
  color: aliceblue;
}
.phone-img {
  display: flex;
  align-items: center;
  justify-content: center;
}
.card {
  background-color: transparent;
  color: white;
}
.num {
  max-width: 80%;
  max-height: 100%;
}

@media screen and (min-width: 150px) and (max-width: 599px) {
  .mx-img {
    max-width: 70% !important;
  }
}
@media screen and (min-width: 600px) and (max-width: 2599px) {
  .mx-img {
    max-width: 400;
  }
}
</style>
