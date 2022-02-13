<template>
  <v-card variant>
    <v-card-header>
      <div>
        <div class="text-overline mb-1">{{category}}</div>
        <div class="text-h6 mb-1">{{title}}</div>
        <div class="text-caption">{{desc}}</div>
      </div>
    </v-card-header>
  </v-card>
</template>

<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
  props: {
    title: {
      type: String,
      default: "",
    },
    category: {
      type: String,
      default: "",
    },
    desc: {
      type: String,
      default: "Greyhound divisely hello coldly fonwderfully",
    },
  },
});
</script>
