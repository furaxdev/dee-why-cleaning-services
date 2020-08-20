<template>
  <div>
    <CFlex justify="space-between" :px="['100px','200px','300px','400px']">
      <div class="brand-logo">
        <c-text font-size="4xl">Dee Why Cleaning Services</c-text>
      </div>

      <themecontroller></themecontroller>
    </CFlex>
  </div>
</template>

<script>
import ThemeToggler from "./chakra/ThemeToggler";
export default {
  inject: ["$chakraColorMode"],
  components: {
    themecontroller: ThemeToggler,
  },
  computed: {
    colorMode() {
      return this.$chakraColorMode;
    },
  },
};
</script>

<style lang="css" scoped>
</style>
