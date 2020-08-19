<template>
  <div>
    <Nuxt />
    <!-- footer ici -->
  </div>
</template>

<style lang="scss">
html {
  font: {
    family: $font-text, -apple-system, BlinkMacSystemFont, sans-serif;
    size: 1em;
  }
  color: $color-grey-9;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

body {
  background-color: $color-grey-1;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}
</style>
