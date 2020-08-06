<template>
  <main class="main">
    <section class="hero">
      <p class="hero__greeting">
        Bonjour !
      </p>
      <p class="hero__introduction">
        Je m'appelle Olivia.
      </p>
      <p class="hero__description">
        Je suis une développeuse Web et Photographe actuellement basée à Nantes.
      </p>
      <!-- Liens vers lers réseaux sociaux-->
      <SocialProfiles />
      <!-- Vers le bas -->
      <div class="hero__CTA--scroll">
        Vers le bas
      </div>
    </section>
  </main>
</template>

<style lang="scss">
.main {
  display: grid;
  grid-template-columns: $spacing-medium auto $spacing-medium;
  padding: $spacing-medium $spacing-xlarge;
}

.hero {
  // display: flex;
  // flex-flow: column nowrap;
  grid-column-start: 2;
  height: 100vh;
  &__greeting {
    font-size: ms(8);
    font-weight: 700;
    letter-spacing: -0.3rem;
    margin-bottom: $spacing-medium;
  }
  &__introduction {
    font-size: ms(6);
    font-weight: 650;
    letter-spacing: -0.1rem;
    color: $color-main;
    margin-bottom: $spacing-medium;
    line-height: $spacing-display-line-height;
  }
  &__description {
    font-size: ms(6);
    font-weight: 160;
    margin-bottom: $spacing-large;
  }
  &__CTA--scroll {
    @extend .ui;
    margin-top: $spacing-large;
  }
}
</style>
