<template>
  <section class="links__socialmedia">
    <a href="https://twitter.com/palingenae" target="_blank" class="link_block">
      Twitter
    </a>
    <a
      href="https://www.instagram.com/palingenae/"
      target="_blank"
      class="link_block"
    >
      Instagram
    </a>
    <a
      href="https://www.github.com/palingenae/"
      target="_blank"
      class="link_block"
    >
      Github
    </a>
  </section>
</template>

<style lang="scss">
.links__socialmedia {
  display: flex;
  flex-flow: row nowrap;
  @media screen and (max-width: 640px) {
    flex-flow: column nowrap;
    align-content: center;
    justify-content: center;
    align-items: center;
    .links__socialmedia:first-child {
      margin: $spacing-small $spacing-medium;
    }
  }
}
</style>

<script>
export default {
  data() {
    return {
      profiles: [
        {
          href: 'https://twitter.com/palingenae',
          icon: 'twitter',
          label: 'Twitter',
        },
        {
          href: 'https://www.instagram.com/palingenae/',
          icon: 'instagram',
          label: 'Instagram',
        },
        {
          href: 'https://www.github.com/palingenae/',
          icon: 'github',
          label: 'Github',
        },
      ],
    }
  },
}
</script>
