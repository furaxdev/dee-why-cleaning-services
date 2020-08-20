<template>
  <div>
    <CBox as="nav" width="100%" :display="{ base: 'none', lg: 'block' }">
      <CStack
        ml="50px"
        spacing="50px"
        as="ul"
        listStyleType="none"
        align="center"
        direction="row"
        color="white"
      >
        <nav-link-item to="/Home" alt="link">Home</nav-link-item>
        <nav-link-item to="/About" alt="link">About</nav-link-item>
        <nav-link-item to="/Contact" alt="link">Contact</nav-link-item>
        <nav-link-item to="/Blog" alt="link">Blog</nav-link-item>
      </CStack>
    </CBox>
  </div>
</template>

<script>
import NavLink from "./NavLink";
export default {
  components: {
    NavLinkItem: NavLink,
  },
};
</script>

<style lang="scss" scoped>
</style>