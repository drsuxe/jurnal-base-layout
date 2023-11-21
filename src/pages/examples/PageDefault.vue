<template>
  <PixelPageContainer>
    <PixelPageHeader title="Title" />
    
    <PixelPageContent variant="card">
      <mp-text>Place content here...</mp-text>
      <mp-input />
    </PixelPageContent>
  </PixelPageContainer>
</template>

<script>
import { MpText, MpInput } from "@mekari/pixel";
import PixelPageContainer from "../../components/wrapper/PixelPageContainer.vue";
import PixelPageContent from "../../components/wrapper/PixelPageContent.vue";
import PixelPageHeader from "../../components/wrapper/PixelPageHeader.vue";

export default {
  components: {
    MpText,
    MpInput,
    PixelPageContainer,
    PixelPageContent,
    PixelPageHeader,
  },
};
</script>
