<template>
  <div>
    <topbar class="z-10"></topbar>
    <div>
      <l-map
        style="height: calc(100vh - 100px)"
        ref="map"
        v-model:zoom="zoom"
        :center="[47.41322, -1.219482]"
      >
        <l-tile-layer
          url="https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png"
          layer-type="base"
          name="OpenStreetMap"
        ></l-tile-layer>
      </l-map>
    </div>
  </div>
</template>

<script>
import { ref, onMounted } from "vue";
import topbar from "@/components/topbarView.vue";
import "leaflet/dist/leaflet.css";
import { LMap, LTileLayer } from "@vue-leaflet/vue-leaflet";

export default {
  name: "HomeView",
  components: {
    topbar,
    LMap,
    LTileLayer,
  },
  setup() {
    const zoom = ref(8);

    onMounted(() => {});

    return {
      zoom,
    };
  },
};
</script>
