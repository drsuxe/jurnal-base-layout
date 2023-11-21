<template>
  <div>
    <PixelNavbar />

    <main
      style="display: flex; height: calc(100vh - var(--jurnal-navbar-height))"
    >
      <PixelSidebar />
      <RouterView />
    </main>

    <PixelLearningCenter />
  </div>
</template>

<script>
import PixelLearningCenter from "./navigation/learning-center/PixelLearningCenter.vue";
import PixelNavbar from "./navigation/navbar/PixelNavbar.vue";
import PixelSidebar from "./navigation/sidebar/PixelSidebar.vue";

export default {
  components: {
    PixelLearningCenter,
    PixelNavbar,
    PixelSidebar,
  },
  mounted() {
    // this.$router.push("/report");
  },
  updated() {
    const element = document.getElementById("jurnal-page-loader");

    if (element) {
      element.remove();
    }
  },
};
</script>

