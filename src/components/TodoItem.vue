
<template>
  <v-list-tile>
    <v-list-tile-content>{{ title }}</v-list-tile-content>
    <v-list-tile-action>
      <div class="“text-xs-center”">
        <v-btn outline color="“indigo”">Done</v-btn>
        <v-btn outline color="“teal”">Delete</v-btn>
      </div>
    </v-list-tile-action>
  </v-list-tile>
</template>

<script>
import { ELOOP } from "constants";
// タイトルと完了したかどうかという状態を持つデータ
export default {
  data() {
    return {
      toggle: "no",
      done: false
    };
  },
  props: {
    title: String
  }
};
</script>