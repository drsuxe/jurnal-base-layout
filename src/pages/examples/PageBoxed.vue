<template>
  <PixelPageContainer>
    <PixelPageHeader title="Layout Boxed" />

    <PixelPageContent variant="blank">
      <mp-simple-grid :columns="[1, 3]" spacing="6" padding-bottom="3">
        <mp-box
          background="white"
          padding="3"
          border-radius="md"
          border-width="1px"
          height="56"
        >
          <mp-text>Place content here...</mp-text>
        </mp-box>
        <mp-box
          background="white"
          padding="3"
          border-radius="md"
          border-width="1px"
          height="56"
        >
          <mp-text>Place content here...</mp-text>
        </mp-box>
        <mp-box
          background="white"
          padding="3"
          border-radius="md"
          border-width="1px"
          height="56"
        >
          <mp-text>Place content here...</mp-text>
        </mp-box>
      </mp-simple-grid>

      <mp-box padding-y="3">
        <mp-box
          background="white"
          padding="3"
          border-radius="md"
          border-width="1px"
          height="56"
        >
          <mp-text>Place content here...</mp-text>
        </mp-box>
      </mp-box>

      <mp-box padding-y="3">
        <mp-box
          background="white"
          padding="3"
          border-radius="md"
          border-width="1px"
          height="56"
        >
          <mp-text>Place content here...</mp-text>
        </mp-box>
      </mp-box>
    </PixelPageContent>
  </PixelPageContainer>
</template>

<script>
import { MpBox, MpText, MpSimpleGrid } from "@mekari/pixel";
import PixelPageContainer from "../../components/wrapper/PixelPageContainer.vue";
import PixelPageContent from "./../components/wrapper/PixelPageContent.vue";
import PixelPageHeader from "./../components/wrapper/PixelPageHeader.vue";

export default {
  components: {
    MpBox,
    MpText,
    MpSimpleGrid,
    PixelPageContainer,
    PixelPageContent,
    PixelPageHeader,
  },
};
</script>
