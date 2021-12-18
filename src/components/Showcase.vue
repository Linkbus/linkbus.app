<template>
    <div class="showcase  mt-3 mt-md-5">
        <b-row class="m-0">
            <b-col order="1" order-md="2" class="text p-sm-0 mx-2">
                <div class="mx-2 mx-lg-4">
                  <h1 class="mt-3 mt-lg-5 m-0 title">Linkbus</h1>
                  <h1 class="mt-1 m-0 sub-title">Fast. Clean. Accurate.</h1>
                  <h1 class="mt-1 m-0 body">View the CSB/SJU Link bus schedule anywhere, anytime from your phone.</h1>
                  <b-row class="m-0 p-0 mt-4" style="align-items: center;">
                      <b-col class="m-0 p-0 mb-4 mr-3" cols="6" sm="5" md="6" lg="4" xl="3">
                          <a href="https://apps.apple.com/us/app/linkbus/id1531257573">
                              <img alt='Get it on the App Store' class="download" src="../assets/Download-on-the-App-Store/US/Download_on_App_Store/Black_lockup/SVG/Download_on_the_App_Store_Badge_US-UK_RGB_blk_092917.svg">
                          </a>
                      </b-col>
                      <b-col class="m-0 p-0 mb-4" cols="6" sm="5" md="6" lg="4" xl="3">
                        <a href='https://play.google.com/store/apps/details?id=com.carroll.michael.linkbus'>
                          <img alt='Get it on Google Play' class="download" src='../assets/google-play.png'/>
                        </a>
                      </b-col>

                  </b-row>
                </div>
            </b-col>

            <b-col cols="9" sm="8" md="5" lg="4" order="2" order-md="1" class="p-sm-0 mx-2">
                <div class="phone mx-3 mx-lg-5">
                    <Phone />
                </div>
            </b-col>
            <b-col cols="12" order="3">

                <div class="wave" style="z-index: 3;">
                    <svg viewBox="0 -110 500 220" class="shape-2">
                        <path d="M500,110 C440,0 240,100
                        0,110 60,220 260,120 500,110 Z"
                              style="stroke: none;
                              fill:#ffffff;">
                        </path>
                    </svg>
                </div>

                <div class="wave" style="z-index: 1;">
                    <svg viewBox="0 0 500 300">
                        <path d="M500,300 C200,300 100,0
                        0,300 L0,300 L500,300 Z"
                              style="stroke: none;
                              fill:#be2136cc;">
                        </path>
                    </svg>
                </div>

                <div class="wave" style="z-index: 2;">
                    <svg viewBox="0 0 500 210">
                        <path d="M500,210 C440,0 240,210
                        0,210 L0,210 L500,210 Z"
                              style="stroke: none;
                              fill:#ffffff80;" >
                        </path>
                    </svg>
                </div>

              <div class="wave" style="z-index: 0;">
                <svg viewBox="0 0 500 210">
                  <path d="M500,210 C440,0 240,210
                        0,210 L0,210 L500,210 Z"
                        style="stroke: none;
                              fill:#be213650;" >
                  </path>
                </svg>
              </div>

            </b-col>
        </b-row>
    </div>
</template>

<script>
    import Phone from './Phone'

    export default {
        name: "Showcase",
        components: {
            Phone
        }
    }
</script>

<style scoped>
    .showcase {
        /*min-height: 100vh;*/
        width: 100%;
    }
    .text {
        z-index: 30;
    }
    .phone {
        position: relative;
        z-index: 2;
    }
    .wave {
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
    }
    .shape-2 {
        overflow: visible;
    }
    .title {
        font-size: 3.5em;
        color: #000000b0;
    }
    .sub-title {
        font-size: 2em;
        color: #000000b0;
    }
    .body {
        font-size: 1.3em;
        color: #000000b0;
    }
    .download {
        width: 100%;
    }
</style>