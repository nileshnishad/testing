<template>
    <div>
        <v-container fluid pa-0 style="background-color: ">
            <v-img
            class="tradebg-img"
            :src="require(`@/assets/media/workSectionBg.webp`)"
            >
              <v-container>
                <v-row>
                  <!-- <v-col cols="12" sm="6" xl="12" class="content mt-10">
                    <v-card-title class="white--text pt-10">
                      <div>
                        <h1>HOW IT WORKS ?</h1>
                      </div>
                      <v-text class="mt-10">
                        <div>
                          Lorem ipsum dolor sit amet consectetur adipisicing elit.
                          Numquam placeat nulla, quam odio error reprehenderit
                          perferendis ducimus corrupti. Dignissimos, vel.
                        </div>
                      </v-text>
                  </v-card-title>
                  </v-col> -->
               </v-row>
                <v-row>
                  <v-col cols="12" sm="6"  xl="6" class="content mt-16" pa-0 >
                    <v-row class="">
                      <v-card-title class="white--text">
                        <div>
                          <h1>HOW IT WORKS ?</h1>
                        </div>
                        <v-text class="mt-8">
                          <div class="main-content">
                            Lorem ipsum dolor sit amet consectetur adipisicing elit.
                            Numquam placeat nulla, quam odio error reprehenderit
                            perferendis ducimus corrupti. Dignissimos, vel.
                          </div>
                        </v-text>
                    </v-card-title>
                      <v-col
                        v-for="title in Work"
                        :key="title.id"
                        cols="12"
                        sm="12"
                        class="mb-3"
                       >
                        <div>
                          <v-card class="card d-flex" elevation="0" title>
                            <v-card-title>
                              <v-flex class="d-flex">
                                <div>
                                  <v-img
                                    :src="require(`@/assets/media/` + title.icon )"
                                    class="mr-10"
                                    max-width="45"
                                  >
                                  </v-img>
                                </div>
                                <div>
                                  <!-- <v-img
                                    :src="require(`@/icon`)"
                                    class="num mr-5"
                                  >
                                  </v-img> -->
                                </div>
                                <div class="main-content">
                                  {{ title.Title }}
                                </div>
                              </v-flex>
                            </v-card-title>
                          </v-card>
                        </div>
                      </v-col>
                    </v-row>
                  </v-col>
                  <v-col cols="12" sm="6"  xl="6" class="mt-16" style="display:flex;align-items:center">
                        <!-- <iframe src="https://www.youtube.com/embed/4FSUCRodPr4"
                        style="width:100%; height:60%; border: 1px solid white;" 
                            title="Guide to Download Fairplay App" frameborder="0" scrolling="no"
                            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                            allowfullscreen="allowfullscreen" ></iframe> -->
                            <iframe width="560" height="315" src="https://www.youtube.com/embed/4FSUCRodPr4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
                  </v-col>
                </v-row>
              </v-container>
            </v-img>
          </v-container>
    </div>
</template>

<script>
    export default {
        data(){
            return{
                Work: [
                {
                    "Title": "Click on WhatsApp",
                    "icon": "work1.webp",
                    "description": "Quick and easy access to your money any time on (FairPlay Share Market?). Avail daily withdrawals and trade faster and better!",
                    "id": 1
                },
                {
                    "Title": "Get in touch with Agent",
                    "icon": "work2.webp",
                    "description": "High market brokerage eating away at your profits? Not anymore! With (FP Share Market?)’s lowest (?) brokerage, your money is all yours!",
                    "id": 2
                },
                {
                    "Title": "Deposit and Get ID",
                    "icon": "work3.webp",
                    "description": "Do away with lengthy account creation and verification troubles with FPSM’s hassle free trading. All you need is to get started and get trading.",
                    "id": 3
                },
                {
                    "Title": "Start Trading",
                    "icon": "work4.webp",
                    "description": "FPSM is your one stop shop for all your trading needs. Find all the popular markets under one roof and gain big profits.",
                    "id": 4
                }
            ],
            }
        }
    }
</script>

<style scoped>
.card {
    background-color: transparent;
    color: white;
    }
.main-content{
    font-family: 'Montserrat', sans-serif;
}
@media only screen and (min-width: 280px) {
  h1{
      font-family: 'Bebas Neue', cursive;
    }
    .v-card__title{
      word-break: break-word;
      line-height: inherit;
    } 
    .main-content{
      font-family: 'Montserrat', sans-serif;
      word-break: break-word;
    }
    h1{
      font-family: 'Bebas Neue', cursive;
    }
    iframe{

    }

    

}
h1{
  font-family: 'Bebas Neue', cursive;
}
.v-card__title{
  word-break: break-word;
  line-height: inherit;
} 
.main-content{
  font-family: 'Montserrat', sans-serif;
  word-break: break-word;
}
h1{
  font-family: 'Bebas Neue', cursive;
}
    
</style>