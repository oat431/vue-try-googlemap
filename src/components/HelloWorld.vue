<template>
  <GoogleMap
    api-key="AIzaSyA6MhxJJLyGPnliSZjaFJb3nJfuroA5Tcw"
    style="width: 100%; height: 500px"
    :center="center"
    :zoom="15"
  >
    <Marker :options="{ position: center }" />
  </GoogleMap>
</template>

<script>
import { GoogleMap, Marker } from "vue3-google-map";

export default {
  components: { GoogleMap, Marker },
  data() {
    return {
      center: { lat: 40.689247, lng: -74.044502 },
    };
  },
};
</script>
