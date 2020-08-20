<template>
  <div class="container">
    <CThemeProvider>
      <CColorModeProvider #default="{ colorMode }">
        <CBox font-family="body" as="main" v-bind="mainStyles[colorMode]" w="100%" minH="100vh">
          <CReset />
          <slot />
        </CBox>
      </CColorModeProvider>
    </CThemeProvider>
  </div>
</template>
<script>

export default {
  mounted() {},
  data() {
    return {
      mainStyles: {
        dark: {
          bg: "gray.700",
          color: "whiteAlpha.900",
        },
        light: {
          bg: "white",
          color: "gray.900",
        },
      },
    };
  },
};
</script>