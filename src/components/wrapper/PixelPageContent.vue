<template>
  <mp-box
    id="pixelPageContent"
    min-height="calc(100vh - 132px)"
    width="full"
    v-bind="{
      ...(variant === 'card' && {
        borderTopWidth: '1px',
        borderLeftWidth: '1px',
        borderTopLeftRadius: 'md',
        borderColor: 'gray.100',
        backgroundColor: 'white',
        padding: 6,
      }),
      ...(variant === 'blank' && {
        borderTopLeftRadius: 'md',
        paddingRight: 6,
        paddingBottom: 6,
      }),
    }"
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
  props: {
    variant: {
      type: String,
      default: "card",
    },
  },
};
</script>
