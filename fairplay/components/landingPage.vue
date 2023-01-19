<template>
    <div>
        <v-container class="main-section1" fluid pa-0>
            <v-img
            :src="require(`@/assets/media/mainBanner.png`)"
            class="main-section1bg"
            >
              <v-container>
                <v-row>
                  <v-card-title class="white--text pt-10">
                  <!-- <h1>Fairplay Market</h1> -->
                  <v-img
                    :src="require(`@/assets/media/logo.png`)"
                    max-height="205"
                    max-width="277"
                  >
                  </v-img>
                </v-card-title>
               </v-row>
                <v-row>
                  <v-col cols="12 " sm="6"  xl="12" class="content">
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
                              <v-flex class="d-flex">
                                <div>
                                  <v-img
                                    :src="require(`@/assets/media/num/Line 8.png`)"
                                    class="mr-5 "
                                  >
                                  </v-img>
                                </div>
                                <div>
                                  <v-img
                                    :src="require(`@/assets/media/num/`+ title.icon )"
                                    class="num mr-5"
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
                    </v-row>
                  </v-col>
                  <v-col cols="12" sm="6" xl="12" class="phone-img">
                    <v-card-title>
                      <v-img
                        
                        :src="require(`@/assets/media/Vector Smart ObjectDWDW.png`)"
                        class="main-section1img"
                      >
                      </v-img>  
                    </v-card-title>
                    <div>'</div>
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
            }
        }
    }
</script>

<style scoped>
section1{
    background: url('@/assets/media/mainBanner.png') no-repeat center center !important;
    background-size: cover;
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
  @media only screen and (min-width: 1024px) {
  .content {
    padding: 30px;
    z-index: 2;
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
  .main-section1{
    position: relative;
    z-index: 1111;
  }
  .main-section1bg{
    position: initial;
  }
  .main-section1img{
    position:absolute;
    z-index: 1;
    bottom: -33px;
    width:470px
  }
  .v-card__title{
    word-break: break-word;
    line-height: inherit;
  } 
  h1{
    font-family: 'Bebas Neue', cursive;
  }
  .main-content{
      font-family: 'Montserrat', sans-serif;
}
  }
  .main-content{
    font-family: 'Montserrat', sans-serif;
    word-break: break-word;
}
@media only screen and (min-width: 300px) {
    h1{
        font-family: 'Bebas Neue', cursive;
      }

}
</style>