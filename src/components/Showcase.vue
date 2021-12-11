<template>
    <div class="showcase  mt-3 mt-md-5">
        <b-row class="m-0">
            <b-col order="1" order-md="2" class="text">
                <h1 class="pl-5 pt-5 m-0 title">Linkbus</h1>
                <h1 class="pl-5 pt-1 m-0 sub-title">Fast. Lightweight. Always accurate.</h1>
                <h1 class="pl-5 pt-1 m-0 body">Easily view the Linkbus schedule anywhere at anytime from your phone.</h1>
                <b-row class="m-0 p-0">
                    <b-col class="m-0 p-0" cols="7" sm="6" md="7" lg="4" xl="3">
                        <a href="https://apps.apple.com/us/app/linkbus/id1531257573">
                            <img class="pl-5 pb-4 pt-4 download" src="../assets/Download-on-the-App-Store/US/Download_on_App_Store/Black_lockup/SVG/Download_on_the_App_Store_Badge_US-UK_RGB_blk_092917.svg">
                        </a>
                    </b-col>
                </b-row>
            </b-col>
            <b-col cols="9" sm="8" md="5" lg="4" order="2" order-md="1">
                <div class="phone ml-5">
                    <Phone />
                </div>
            </b-col>
            <b-col cols="12" order="3">
<!--                <div class="wave" style="background: red">-->

<!--                </div>-->
                <div class="wave" style="z-index: 5;">
                    <svg viewBox="0 -110 500 220" class="shape-2">

<!--                        <path d="M0, 0 C60, 110 260,-->
<!--                0 500, 0 L500, 00 L0, 0 Z"-->
<!--                        <path d="M500, 0 C440, 110 240,-->
<!--                0 0, 0 L0,0 L500,0 Z"-->
<!--                        <path d="M500,110 C440,0 240,100-->
<!--                        0,110 L0,110 L500,110 Z"-->
                        <path d="M500,110 C440,0 240,100
                        0,110 60,220 260,120 500,110 Z"
                              style="stroke: none;
                fill:rgba(142, 199, 240, 1.0);">
                        </path>
                    </svg>
                </div>

                <div class="wave" style="z-index: 1;">
                    <svg viewBox="0 0 500 300">
                        <path d="M500,300 C200,300 100,0
                        0,300 L0,300 L500,300 Z"
                              style="stroke: none;
                fill:rgba(153, 50, 204, 0.5);">
                        </path>
                    </svg>
                </div>

                <div class="wave" style="z-index: 4;">
                    <svg viewBox="0 0 500 210">
                        <path d="M500,210 C440,0 240,210
                        0,210 L0,210 L500,210 Z"
                              style="stroke: none;
                fill:rgba(255, 255, 254, 0.7);" >
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
        font-size: 1em;
        color: #000000b0;
    }
    .download {
        width: 100%;
    }
</style>