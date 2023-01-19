<template>
  
  <v-app>
    <!-- logo and landing first section  -->
    <v-container fluid pa-0>
      <v-img
        :src="require(`@/assets/media/mainBanner.png`)"
       
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
                              class="mr-10 pa-1"
                            >
                            </v-img>
                          </div>
                          <div>
                            <v-img
                              :src="require(`@/assets/media/num/01.png`)"
                              class="num mr-5"
                            >
                            </v-img>
                          </div>
                          <div>
                            {{ title.Title }}
                          </div>
                        </v-flex>
                      </v-card-title>
                    </v-card>
                  </div>
                </v-col>
              </v-row>
            </v-col>
            <v-col cols="12" sm="6" xl="12">
              <v-card-title>
                <v-img
                  :src="require(`@/assets/media/Vector Smart ObjectDWDW.png`)"
                >
                </v-img>  
              </v-card-title>
              <div>'</div>
            </v-col>
          </v-row>
        </v-container>
      </v-img>
    </v-container>
    
    <!-- 2nd section -->
    <v-container fluid pa-0 style="background-color: #07083a">
      <v-img
        :src="require(`@/assets/media/section2bg.png`)"
       
      >
        <v-container>
          <v-row>
            <v-col cols="12" sm="6" xl="12" class="content mt-10">
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
            </v-col>
         </v-row>
          <v-row>
            <v-col cols="12" sm="6"  xl="6" class="content">
              <v-row class="mt-2">
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
                              :src="require(`@/assets/media/num/Line 8.png`)"
                              class="mr-10 pa-1"
                            >
                            </v-img>
                          </div>
                          <div>
                            <v-img
                              :src="require(`@/assets/media/num/01.png`)"
                              class="num mr-5"
                            >
                            </v-img>
                          </div>
                          <div>
                            {{ title.Title }}
                          </div>
                        </v-flex>
                      </v-card-title>
                    </v-card>
                  </div>
                </v-col>
              </v-row>
            </v-col>
            <v-col cols="6" sm="6"  xl="6">
                  <iframe src="https://www.youtube.com/embed/4FSUCRodPr4"
                  style="width:100%; height:100%" 
                      title="Guide to Download Fairplay App" frameborder="0" scrolling="no"
                      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                      allowfullscreen="allowfullscreen" ></iframe>
                    
            </v-col>
          </v-row>
        </v-container>
      </v-img>
    </v-container>
    <!-- <v-container fluid pa-0 style="background-color: #07083a">
      <v-img
        :src="require(`@/assets/media/section2bg.png`)"
        
      >
        <v-container>
          <v-row no-gutters>
            <v-col cols="12" sm="6" class="content mt-10">
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

              <v-row class="mt-15">
                <v-col
                  v-for="title in Work"
                  :key="title.id"
                  cols="12"
                  sm="12"
                  class="mb-10"
                >
                  <div>
                    <v-card class="card d-flex" elevation="0" title>
                      <v-card-title>
                        <v-flex class="d-flex">
                          <div>
                            <v-img
                              :src="require(`@/assets/media/num/Line 8.png`)"
                              class="mr-10 pa-1"
                            >
                            </v-img>
                          </div>
                          <div>
                            <v-img
                              :src="require(`@/assets/media/num/01.png`)"
                              class="num mr-5"
                            >
                            </v-img>
                          </div>
                          <div>
                            {{ title.Title }}
                          </div>
                        </v-flex>
                      </v-card-title>
                    </v-card>
                  </div>
                </v-col>
              </v-row>
            </v-col>
            <v-col cols="12" sm="6" class="mt-10">
              <v-card-title>
                <h1>hii</h1>
              </v-card-title>
            </v-col>
          </v-row>
        </v-container>
      </v-img>
    </v-container> -->
    <!-- 3rd section -->
    <v-container fluid pa-0>
      <v-img :src="require(`@/assets/media/section3bg.png`)">
        <v-container>
          <v-row no-gutters>
            <v-col cols="12" sm="6" class="content mt-10">
              <v-card-title class="white--text pt-10">
                <div>
                  <h1>GET YOUR DEMO ID</h1>
                </div>
                <v-text class="mt-10">
                  <div>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Numquam placeat nulla, quam odio error reprehenderit
                    perferendis ducimus corrupti. Dignissimos, vel.
                  </div>
                </v-text>
                <div>
                  <v-btn>h111</v-btn>
                  <v-btn>h111</v-btn>

                </div>
              </v-card-title>
            </v-col>

            <v-col cols="12" sm="6">
              <v-img
                :src="require(`@/assets/media/Design.png`)"
                max-width="300"
                class="ml-16"
              >
              </v-img>
            </v-col>
          </v-row>
        </v-container>
      </v-img>
    </v-container>

    <!-- 4th section -->
    <v-container fluid pa-0>
      <v-img :src="require(`@/assets/media/section4bg.png`)">
        <v-container>
          <v-row no-gutters>
            <v-col
              cols="12"
              sm="6"
              class="d-flex"
              style="align-items: center"
            >
              <v-img
                :src="require(`@/assets/media/Vector Smart ObjectCSC.png`)"
                max-width="300"
                class="ml-16"
              >
              </v-img>
            </v-col>
            <v-col cols="12" sm="6" class="content mt-10">
              <v-card-title class="white--text pt-10">
                <v-text>
                  <h1>GET AN ID INSTANTLY ON WHATSAPP</h1>
                </v-text>
                <v-text class="mt-5">
                  <h3>Get in touch with our customer care</h3>
                </v-text>
                <v-text class="mt-5">
                  <h4>Lorem ipsum dolor sit amet consectetur adipisicing elit. Officia dignissimos eos ipsa error sed rem.</h4>
                </v-text>
                <v-text class="mt-5">
                  <h4>Whatsapp us on</h4>
                  <v-btn>+91 99988 888888</v-btn>
                </v-text>
                <v-text class="mt-5">
                  <h4>With our step-by-step guide for beginners</h4>
                  <v-btn>+91 99988 99988</v-btn>
                </v-text>
                <v-text class="">

                </v-text>
                <v-text class="mt-10">
                  <div>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Numquam placeat nulla, quam odio error reprehenderit
                    perferendis ducimus corrupti. Dignissimos, vel.
                  </div>
                </v-text>
              </v-card-title>
            </v-col>
          </v-row>
        </v-container>
      </v-img>
    </v-container>

  </v-app>
  
</template>

<script>
export default {
name: "IndexPage",
data() {
  return {
    Data: [],
    Work: [],
  };
},
created() {
  this.data();
  this.work();
},
methods: {
  async data() {
    await fetch("http://localhost:8080/data")
      .then((response) => {
        if (response.ok) {
          return response.json();
        }
      })
      .then((data) => {
        this.Data = data;

        // this.title = Data.Title
        console.log(this.Data);

        // console.log(this.title)
      });
  },
  async work() {
    await fetch("http://localhost:8080/work")
      .then((response) => {
        if (response.ok) {
          return response.json();
        }
      })
      .then((data) => {
        this.Work = data;

        // this.title = Data.Title
        console.log(this.Work);

        // console.log(this.title)
      });
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
@media only screen and (min-width: 1024px) {
.content {
  padding: 30px;
}
}
</style>
