<template>
  <v-app>
    <app-bar />
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import appBar from "@/components/common/appBar.vue";

export default defineComponent({
  name: "App",
  components: { appBar },
  data() {
    return {
      //
    };
  },
});
</script>
