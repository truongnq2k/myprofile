<template>
  <v-app>
    <!-- <Header /> -->
    <router-view></router-view>
    <!-- <Sidebar /> -->
    <Footer />
  </v-app>
</template>

<script>
// import Header from "@/components/Header";
import Footer from "@/components/Footer";
// import Sidebar from "@/components/Sidebar";

export default {
  name: "App",

  components: {
    // Header,
    Footer,
    //Sidebar
  },

  data: () => ({
    //
  }),
};
</script>

