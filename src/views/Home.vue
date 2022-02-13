<template>
  <itemList />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import itemList from "../components/list.vue";

export default defineComponent({
  name: "Home",

  components: {
    itemList,
  },
});
</script>
