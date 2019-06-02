<template>
  <v-list-tile>
    <v-list-tile-content>{{ title }}</v-list-tile-content>
    <v-list-tile-action>
      <input type="checkbox" v-model="toggle" true-value="yes" false-value="no">
    </v-list-tile-action>
  </v-list-tile>
</template>

<script>
export default {
  data() {
    return {
      toggle: "no"
    };
  },
  props: {
    title: String
  }
};
</script>
