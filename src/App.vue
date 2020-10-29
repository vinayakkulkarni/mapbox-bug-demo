<template>
  <div id="app">
    <MglMap class="mglmap" container="map" :zoom="10.5" :access-token="accessToken" :map-style="mapStyle" :center="sgCenter">
    </MglMap>
  </div>
</template>

<script>
import 'mapbox-gl/dist/mapbox-gl.css'
// import Mapbox from "mapbox-gl"
import { MglMap } from "v-mapbox"

export default {
  name: 'App',
  components: {
    MglMap
  },
  data(){
    return {
      accessToken: '', // Enter your own access token
      mapStyle: 'mapbox://styles/mapbox/dark-v9',
      sgCenter: [103.82161, 1.35433],
    };
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
