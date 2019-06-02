<template>
  <v-app>
    <Header></Header>
  </v-app>
</template>

<script>
import Footer from "./components/Footer";
import Header from './components/Header'

export default {
  name: "App",
  components: {
    Footer
    Header
  },
  data() {
    return {
      //
    };
  }
};
</script>
