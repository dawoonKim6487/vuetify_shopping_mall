<template>
  <v-list density="compact">
    <v-list-subheader>Sale items</v-list-subheader>
    <v-list-item v-for="(item, i) in items" :key="i" :value="item" active-color="primary">
      <listItem />
      <v-list-item-title v-text="item.text"></v-list-item-title>-->
    </v-list-item>
  </v-list>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import listItem from "./list_item.vue";

export default defineComponent({
  components: { listItem },
  data() {
    return {
      items: [
        { titel: "Lorem ipsum", text: "Real-Time", icon: "mdi-clock" },
        { titel: "Lorem ipsum", text: "Audience", icon: "mdi-account" },
        { titel: "Lorem ipsum", text: "Conversions", icon: "mdi-flag" },
        { titel: "Lorem ipsum", text: "Conversions", icon: "mdi-flag" },
        { titel: "Lorem ipsum", text: "Conversions", icon: "mdi-flag" },
        { titel: "Lorem ipsum", text: "Conversions", icon: "mdi-flag" },
        { titel: "Lorem ipsum", text: "Conversions", icon: "mdi-flag" },
      ],
    };
  },
});
</script>