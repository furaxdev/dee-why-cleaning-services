<template>
  <div>
    <CPseudoBox
      as="li"
      color="white"
      :fontSize="{ base: 'sm', lg: 'md' }"
      fontWeight="medium"
      fontFamily="Kelson"
      textTransform="uppercase"
      position="relative"
      cursor="pointer"
    >
      <c-text
        as="nuxt-link"
        font-family="Kelson,system-ui,Helvetica,sans-serif"
        font-weight="normal"
        :to="to"
      >
        <slot />
      </c-text>
    </CPseudoBox>
  </div>
</template>

<script>
export default {
  props: {
    to: {
      type: String,
      default: "#",
    },
  },
};
</script>

<style lang="scss" scoped>
</style>