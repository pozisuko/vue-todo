<template>
  <v-app>
    <Header></Header>
    <Footer></Footer>
  </v-app>
</template>

<script>
import Footer from "./components/Footer";
import Header from './components/Header';

export default {
  name: "App",
  components: {
    Footer,
    Header
  },
  data() {
    return {
      //
    };
  }
};
</script>
