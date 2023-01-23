<template>
  <div>
    <v-container fluid pa-0>
      <v-img :src="require(`@/assets/media/whatsappSection.webp`)">
        <v-container>
          <v-row no-gutters>
            <v-col cols="12" sm="6" class="d-flex" style="align-items: center">
              <v-img
                :src="require(`@/assets/media/Vector-Smart-ObjectCSC.webp`)"
                max-width="381"
                class="whatsapp_img"
              >
              </v-img>
            </v-col>
            <v-col cols="12" sm="6" class="content">
              <v-card-title class="white--text">
                <v-text>
                  <div class="whatsapp-div">
                    <v-img
                      :src="
                        require(`@/assets/media/Vector-Smart-ObjectCSC.webp`)
                      "
                      max-width="60"
                      class="mobile_whatsapp_img mr-3"
                    />
                  </div>
                </v-text>
                <div>
                  <h1>WE’D LOVE TO HEAR FROM YOU</h1>
                </div>
                <v-text>
                  <h4>
                    Do you have questions or suggestions? Our dedicated customer
                    care team is at your service. For all queries, feedback or
                    complaints, contact our agents on : ______
                  </h4>
                </v-text>
                <v-text class="mt-5">
                  <h4>Whatsapp us on</h4>
                  <v-hover v-slot="{ hover }">
                    <v-btn
                      class="rounded-0 pt-7 pb-7"
                      outlined
                      :style="{
                        'background-color': hover ? 'green' : 'transparent',
                      }"
                    >
                      +44 7938 438723
                    </v-btn>
                  </v-hover>
                </v-text>
                <v-text class="mt-5">
                  <h4>With our step-by-step guide for beginners</h4>
                  <v-hover v-slot="{ hover }">
                    <v-btn
                      class="rounded-0 pt-7 pb-7"
                      outlined
                      :style="{
                        'background-color': hover ? 'green' : 'transparent',
                      }"
                    >
                      +44 7938 438723
                    </v-btn>
                  </v-hover>
                </v-text>
              </v-card-title>
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
  .main-section1 {
    position: relative;
    z-index: 1111;
  }
  .main-section1bg {
    position: initial;
  }
  .main-section1img {
    position: absolute;
    z-index: 1;
    bottom: -33px;
  }
  .v-card__title {
    word-break: break-word;
    line-height: inherit;
  }
  h1 {
    font-family: "Bebas Neue", cursive;
  }
}
@media only screen and (min-width: 280px) {
  h1 {
    font-family: "Bebas Neue", cursive;
  }
  .v-card__title {
    word-break: break-word;
    line-height: inherit;
  }
}
.whatsapp-div {
  float: left;
  height: 150px;
}

.mobile_whatsapp_img {
  float: left;
}
.whatsapp_img {
  padding: 0px;
  width: 30%;
}
@media screen and (min-width: 150px) and (max-width: 599px) {
  .whatsapp_img {
    display: none;
  }
}
@media screen and (min-width: 600px) and (max-width: 2200px) {
  .mobile_whatsapp_img {
    display: none;
  }
}
</style>
