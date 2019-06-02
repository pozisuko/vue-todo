<template>
  <v-list-tile v-if="!done">
    <v-list-tile-content>{{ title }}</v-list-tile-content>
    <v-list-tile-action>
      <div class="text-xs-center">
        <v-btn outline color="success" @click="done=!done">Done</v-btn>
      </div>
    </v-list-tile-action>
  </v-list-tile>
</template>

<script>
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