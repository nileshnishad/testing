<template>
  <div>
    <v-container fluid pa-0 style="background-color: ">
      <v-img
        class="tradebg-img"
        :src="require(`@/assets/media/workSectionBg.webp`)"
      >
        <v-container>
          <v-row>
            <v-col cols="12" sm="6" xl="6" class="content mt-5 pa-0" pa-0>
              <v-card-title class="white--text">
                <div>
                  <h1>HOW IT WORKS ?</h1>
                </div>
              </v-card-title>
              <v-col
                v-for="title in Work"
                :key="title.id"
                cols="12"
                sm="12"
                class=""
              >
                <div>
                  <v-card class="card d-flex" elevation="0" title>
                    <v-card-title>
                      <v-flex class="d-flex">
                        <div>
                          <v-img
                            :src="require(`@/assets/media/` + title.icon)"
                            class="mr-5"
                            max-width="40"
                          >
                          </v-img>
                        </div>
                        <div class="main-content">
                          {{ title.Title }}
                        </div>
                      </v-flex>
                    </v-card-title>
                  </v-card>
                </div>
              </v-col>
            </v-col>
            <v-col
              cols="12"
              sm="6"
              xl="6"
              class="mt-1 mb-3 video-frame d-flex justify-content-center"
            >
              <iframe
                width="80%"
                height="80%"
                class="i_frame"
                src="https://fairplay-image.fairplay.co.in/landing-promotion.mp4"
                title="YouTube video player"
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                allowfullscreen
                frameBorder="0"
              ></iframe>
            </v-col>
          </v-row>
        </v-container>
      </v-img>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      Work: [
        {
          Title: "Click on the Whatsapp Icon",
          icon: "work1.webp",
          description:
            "Quick and easy access to your money any time on (FairPlay Share Market?). Avail daily withdrawals and trade faster and better!",
          id: 1,
        },
        {
          Title: "An agent will be assigned to you",
          icon: "work2.webp",
          description:
            "High market brokerage eating away at your profits? Not anymore! With (FP Share Market?)’s lowest (?) brokerage, your money is all yours!",
          id: 2,
        },
        {
          Title: "Deposit & Create ID",
          icon: "work3.webp",
          description:
            "Do away with lengthy account creation and verification troubles with FPSM’s hassle free trading. All you need is to get started and get trading.",
          id: 3,
        },
        {
          Title: "Start trading and making profits",
          icon: "work4.webp",
          description:
            "FPSM is your one stop shop for all your trading needs. Find all the popular markets under one roof and gain big profits.",
          id: 4,
        },
      ],
    };
  },
};
</script>

<style scoped>
h1 {
  font-family: "Bebas Neue", cursive;
}
.card {
  background-color: transparent;
  color: white;
}
.v-card__title {
  word-break: break-word;
  line-height: inherit;
}
.main-content {
  font-family: "Montserrat", sans-serif;
  word-break: break-word;
}
.video-frame {
  align-items: center;
}
.i_frame {
  width: 100%;
  height: 100%;
  align-items: center;
}
</style>
