<template>
  <nav class="navigation__site">
    <div class="navigation__elements">
      <a class="navigation__link">#À propos</a>
      <a class="navigation__link">#Projets</a>
      <a class="navigation__link">#Say Hi</a>
    </div>
  </nav>
</template>

<style lang="scss">
.navigation {
  &__site {
    display: flex;
    flex-flow: row nowrap;
    justify-content: flex-end;
    padding: $spacing-medium $spacing-xlarge;
  }
  &__link {
    font-weight: 500;
    padding: $spacing-small $spacing-medium;
  }
}
</style>
