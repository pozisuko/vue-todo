<template>
  <v-app>
    <Header></Header>
    <TodoIterator></TodoIterator>
    <Footer></Footer>
  </v-app>
</template>

<script>
import Footer from "./components/Footer";
import Header from "./components/Header";
import TodoIterator from "./components/TodoIterator";

export default {
  name: "App",
  components: {
    Footer,
    Header,
    TodoIterator
  },
  data() {
    return {
      //
    };
  }
};
</script>
