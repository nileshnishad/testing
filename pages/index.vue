<template>
  
  <v-app>
    <LandingPage/>
    <WorkSection/>
    <demoIdSection/>
    <whatsappSection/>
    
  </v-app>
  
</template>

<script>
import LandingPage from '../components/landingPage.vue';
import WorkSection from '../components/workSection.vue';

export default {
    name: "IndexPage",
    data() {
        return {
            Data: [
                {
                    "Title": "No Commission",
                    "icon": "01.png",
                    "description": "Quick and easy access to your money any time on (FairPlay Share Market?). Avail daily withdrawals and trade faster and better!",
                    "id": 1
                },
                {
                    "Title": "No DEMAT and KYC required",
                    "icon": "02.png",
                    "description": "High market brokerage eating away at your profits? Not anymore! With (FP Share Market?)’s lowest (?) brokerage, your money is all yours!",
                    "id": 2
                },
                {
                    "Title": "Low brokerage",
                    "icon": "03.png",
                    "description": "Do away with lengthy account creation and verification troubles with FPSM’s hassle free trading. All you need is to get started and get trading.",
                    "id": 3
                },
                {
                    "Title": "Low MCX/NSC/COMX markets available",
                    "icon": "04.png",
                    "description": "FPSM is your one stop shop for all your trading needs. Find all the popular markets under one roof and gain big profits.",
                    "id": 4
                }
            ],
            Work: [
                {
                    "Title": "Click on WhatsApp",
                    "icon": "work1.png",
                    "description": "Quick and easy access to your money any time on (FairPlay Share Market?). Avail daily withdrawals and trade faster and better!",
                    "id": 1
                },
                {
                    "Title": "Get in touch with Agent",
                    "icon": "work2.png",
                    "description": "High market brokerage eating away at your profits? Not anymore! With (FP Share Market?)’s lowest (?) brokerage, your money is all yours!",
                    "id": 2
                },
                {
                    "Title": "Deposit and Get ID",
                    "icon": "work3.png",
                    "description": "Do away with lengthy account creation and verification troubles with FPSM’s hassle free trading. All you need is to get started and get trading.",
                    "id": 3
                },
                {
                    "Title": "Start Trading",
                    "icon": "work4.png",
                    "description": "FPSM is your one stop shop for all your trading needs. Find all the popular markets under one roof and gain big profits.",
                    "id": 4
                }
            ],
        };
    },
    // created() {
    //     this.data();
    //     this.work();
    // },
    // methods: {
    //     async data() {
    //         await fetch("http://localhost:8080/data")
    //             .then((response) => {
    //             if (response.ok) {
    //                 return response.json();
    //             }
    //         })
    //             .then((data) => {
    //             this.Data = data;
    //             // this.title = Data.Title
    //             console.log(this.Data);
    //             // console.log(this.title)
    //         });
    //     },
    //     async work() {
    //         await fetch("http://localhost:8080/work")
    //             .then((response) => {
    //             if (response.ok) {
    //                 return response.json();
    //             }
    //         })
    //             .then((data) => {
    //             this.Work = data;
    //             // this.title = Data.Title
    //             console.log(this.Work);
    //             // console.log(this.title)
    //         });
    //     },
    // },
    components: { LandingPage, WorkSection }
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
@media only screen and (min-width: 1024px) {
.content {
  padding: 30px;
  z-index: 2;
}
.phone-img{
 
}
.tradebg-img{
  z-index: 1;
}
.bg3{
  z-index: 1;
}
.hand-img{
  z-index:2;
}
.main-section3{
  position: relative;
  z-index: 1111;
}
.main-section3bg{
  position: initial;
}
.main-section3img{
  position:absolute;
  z-index: 1;
  bottom: -33px
}
.v-card__title{
  word-break: break-word;
  line-height: inherit;
} 
h1{
  font-family: 'Bebas Neue', cursive;
}
}
</style>
