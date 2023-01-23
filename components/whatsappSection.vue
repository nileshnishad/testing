<template>
  <div>
    <v-container fluid pa-0>
      <v-img :src="require(`@/assets/media/whatsappSection.webp`)">
        <v-container class="mt-4">
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
              <div class="whatsapp-div mt-7">
                <v-img
                  :src="require(`@/assets/media/Vector-Smart-ObjectCSC.webp`)"
                  max-width="60"
                  class="mobile_whatsapp_img mr-3"
                />
              </div>

              <div class="mt-5 d-flex">
                <h1>WE’D LOVE TO HEAR FROM YOU</h1>
              </div>
              <v-text>
                <p class="mt-5">
                  Do you have questions or suggestions? Our dedicated customer
                  care team is at your service. For all queries, feedback or
                  complaints, contact our agents on : ______
                </p>
              </v-text>
              <v-text class="mt-5">
                <h4>Whatsapp us on</h4>
                <v-hover v-slot="{ hover }">
                  <v-btn
                    class="rounded-0 pt-7 pb-7 mt-2 mb-5"
                    outlined
                    :style="{
                      'background-color': hover ? 'green' : 'transparent',
                    }"
                  >
                    +44 7938 438723
                  </v-btn>
                </v-hover>
              </v-text>
              <v-text class="mt-10">
                <h4>With our step-by-step guide for beginners</h4>
                <v-hover v-slot="{ hover }">
                  <v-btn
                    class="rounded-0 pt-7 pb-7 mt-2 mb-5"
                    outlined
                    :style="{
                      'background-color': hover ? 'green' : 'transparent',
                    }"
                  >
                    +44 7938 438723
                  </v-btn>
                </v-hover>
              </v-text>
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
  h1 {
    font-family: "Bebas Neue", cursive;
  }
}
.whatsapp-div {
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
