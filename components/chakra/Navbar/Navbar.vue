<template>
  <div>
    <c-grid
      :template-columns="['1fr','4fr 10fr']"
      :py="['10px','20px']"
      gap="6"
      :h="['50px', '70px']"
      bg="#323c34"
      color="white"
    >
      <div class="brand-logo">
        <c-text
          font-size="1.5rem"
          font-family="Kelson,system-ui,Helvetica,sans-serif"
          textTransform="uppercase"
        >Dee Why</c-text>
      </div>

      <navigation-links></navigation-links>
    </c-grid>
  </div>
</template>

<script>
import NavLinks from "./NavLinks";
export default {
  components: {
    NavigationLinks: NavLinks,
  },
};
</script>

<style lang="css" scoped>
</style>
