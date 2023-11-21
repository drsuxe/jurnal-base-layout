<template>
  <mp-box
    id="pixelPageContainer"
    as="section"
    width="100%"
    background-color="background"
    height="calc(100vh - var(--jurnal-navbar-height))"
    overflow-y="auto"
  >
    <slot />
  </mp-box>
</template>

<script>
import { MpBox } from "@mekari/pixel";
export default {
  components: {
    MpBox,
  },
};
</script>
