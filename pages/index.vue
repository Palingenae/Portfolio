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
      <!-- <div class="hero__CTA--scroll">
        <font-awesome-icon icon="arrow-down" />
        Vers le bas
      </div> -->
    </section>
    <!-- <section class="projects">
      <h2>Mes projets</h2>
    </section> -->
  </main>
</template>

<style lang="scss">
.main {
  // display: grid;
  // grid-template-columns: $spacing-medium auto $spacing-medium;
  display: flex;
  align-content: center;
  align-items: center;
  padding: $spacing-xlarge;
  height: 100vh;
  @media screen and (max-width: 1024px) {
    padding: $spacing-large;
  }
  @media screen and (max-width: 640px) {
    padding: $spacing-medium;
    align-content: flex-start;
    align-items: flex-start;
  }
}

.hero {
  display: flex;
  flex-flow: column nowrap;
  // grid-column-start: 2;
  // height: 100vh;
  max-width: 64rem;
  &__greeting {
    @extend .jumbo;
    font-weight: 700;
    letter-spacing: -0.3rem;
    margin-bottom: $spacing-medium;
  }
  &__introduction {
    @extend h2;
    font-weight: 700;
    letter-spacing: -0.1rem;
    color: $color-main;
    margin-bottom: $spacing-medium;
    line-height: $spacing-display-line-height;
  }
  &__description {
    @extend h2;
    font-weight: 160;
    margin-bottom: $spacing-large;
    line-height: $spacing-display-line-height;
  }
  &__CTA--scroll {
    // @extend .ui;
    margin-top: $spacing-large;
  }
}

.projects {
  grid-column-start: 2;
}
</style>
