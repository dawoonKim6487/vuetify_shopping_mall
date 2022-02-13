<template>
  <v-list density="compact">
    <v-card-title class="text-xs-h6 text-md-h5 text-lg-h4">판매 리스트</v-card-title>
    <v-list-item v-for="(item, i) in items" :key="i" :value="item" active-color="primary">
      <listItem :title="item.title" :category="item.category" :desc="item.text" />
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
        {
          category: "티셔츠",
          title: "판매품목1",
          text: "Greyhound divisely hello coldly fonwderfully",
          icon: "mdi-clock",
        },
        {
          category: "신발",
          title: "판매품목2",
          text: "Lorem sit velit adipisicing minim non esse officia minim culpa tempor.",
          icon: "mdi-account",
        },
        {
          category: "데님",
          title: "판매품목3",
          text: "Greyhound divisely hello coldly fonwderfully",
          icon: "mdi-flag",
        },
        {
          category: "면바지",
          title: "판매품목4",
          text: "Mollit fugiat minim laborum nisi veniam eu labore culpa aliqua dolore voluptate.",
          icon: "mdi-flag",
        },
        {
          category: "기타",
          title: "판매품목5",
          text: "Greyhound divisely hello coldly fonwderfully",
          icon: "mdi-flag",
        },
        {
          category: "슬랙스",
          title: "판매품목6",
          text: "Minim et labore ea veniam cupidatat consectetur proident voluptate eu cillum est cupidatat dolore.",
          icon: "mdi-flag",
        },
        {
          category: "아우터",
          title: "판매품목7",
          text: "Greyhound divisely hello coldly fonwderfully",
          icon: "mdi-flag",
        },
      ],
    };
  },
});
</script>