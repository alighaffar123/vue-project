<template>
  <div class="map-section">
    <div class="container">
      <div class="map-grid shadow-lg bg-white">
        <div class="map">
          <GoogleMap
              api-key="AIzaSyCZcLipUHRw-52ddpIL6bHLAW9Q5nfYvzo"
              class="map-style"
              :center="center"
              :zoom="15"
              >
              <Marker :options="{ position: center }" />
          </GoogleMap>
        </div>
        <div class="moniter p-3">
            <div class="sales position-relative">
                <a href="">
                    <fa icon="xmark" class="xmark "/>
                </a>
                <div class="text">
                     <h5>
                    SALES MONITER
                </h5>
                <p>
                    Easyto review sales  activies by the world map to the improve markit planing
                </p>
                </div>
            </div>
          <div class="mb-auto circle d-flex justify-content-center align-items-center">
           <div class="left">
             <div class="c100 p25">
              <span>25%</span>
              <div class="slice">
                <div class="bar"></div>
                <div class="fill"></div>
              </div>
            </div>
            <p class="text-center">United State</p>
           </div>

           <div class="center">
             <div class="c100 p25">
              <span>50%</span>
              <div class="slice">
                <div class="bar"></div>
                <div class="fill"></div>
              </div>
            </div>
            <p class="text-center">United State</p>
           </div>

           <div class="right">
             <div class="c100 p25">
              <span>25%</span>
              <div class="slice">
                <div class="bar"></div>
                <div class="fill"></div>
              </div>
            </div>
            <p class="text-center">United State</p>
           </div>

          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { defineComponent } from 'vue'
import { GoogleMap, Marker } from 'vue3-google-map'

export default defineComponent({
  name:"vue-map",
  components: { GoogleMap, Marker },
  setup() {
    const center = { lat: 40.689247, lng: -74.044502 }

    return { center }
  },
})
</script>

<style lang="scss" scoped>
@import '/src/assets/scss/component/map.scss';
</style>