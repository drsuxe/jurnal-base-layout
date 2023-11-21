<template>
    <PageWithTab v-if="$route.path === '/report'" />
    <PageDefault v-else />
</template>

<script>
import PageWithTab from "./examples/PageWithTab.vue";
import PageDefault from './examples/PageDefault.vue'
export default {
  components: {
    PageWithTab,
    PageDefault
  },
};
</script>
