<template>
  <div>
    <CIconButton
      mr="3"
      :icon="colorMode === 'light' ? 'moon' : 'sun'"
      :aria-label="`Switch to ${
              colorMode === 'light' ? 'dark' : 'light'
            } mode`"
      @click="toggleColorMode"
    />
  </div>
</template>

<script lang="js">


export default {

  inject: ['$chakraColorMode', '$toggleColorMode'],
  computed: {
    colorMode () {
      return this.$chakraColorMode()
    },
    theme () {
      return this.$chakraTheme()
    },
    toggleColorMode () {
      return this.$toggleColorMode
    }
  },

}
</script>
