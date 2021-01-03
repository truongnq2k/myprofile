<template>
  <div class="home">
    <Banner />
    <div class="container">
      <v-alert class="mt-3" outlined type="success" text
        >Một sản phẩm còn sống còn phải sửa còn phải code... Sản phẩm gọi là
        xong thì là sản phẩm đã chết, không có khái niệm code xong
      </v-alert>
      <Timeline />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Timeline from "@/components/Timeline";
import Banner from "@/components/Banner";
export default {
  name: "Home",
  components: { Timeline, Banner },
  created() {
    document.title = "Tdevs by Quang Truong";
  },
};
</script>
