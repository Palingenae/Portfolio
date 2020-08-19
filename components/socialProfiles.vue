<template>
  <section class="links__socialmedia">
    <a href="" target="_blank" class="link_block">
      <span class="link__label">Twitter</span>
    </a>
    <a href="" target="_blank" class="link_block">
      <fa :icon="['fab', 'instagram']" />
      <span class="link__label">Instagram</span>
    </a>
    <a href="" target="_blank" class="link_block">
      <font-awesome-icon :icon="['fab', 'FaIconGithub']" />
      <span class="link__label">Github</span>
    </a>
  </section>
</template>

<script>
export default {
  data() {
    return {
      profiles: [
        {
          href: 'https://twitter.com/palingenae',
          linkClass: 'link_block link__branded--twitter',
          icon: 'twitter',
          label: 'Twitter',
        },
        {
          href: 'https://www.instagram.com/palingenae/',
          linkClass: 'link_block link__branded--instagram',
          icon: 'instagram',
          label: 'Instagram',
        },
        {
          href: 'https://www.github.com/palingenae/',
          linkClass: 'link_block link__branded--github',
          icon: 'github',
          label: 'Github',
        },
      ],
    }
  },
}
</script>
