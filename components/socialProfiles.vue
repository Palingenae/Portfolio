<template>
  <section class="links--socialmedia">
    <a
      v-for="profile in profiles"
      :key="profile.label"
      :href="profile.href"
      target="_blank"
      :class="profile.linkClass"
    >
      <i :class="profile.icon" />
      <span class="link__label">{{ profile.label }}</span>
    </a>
  </section>
</template>

<script>
export default {
  data() {
    return {
      profiles: [
        {
          href: 'https://twitter.com/palingenaes',
          linkClass: 'link_block link__branded--twitter',
          icon: 'fab fa-twitter',
          label: 'Twitter',
        },
        {
          href: 'https://www.instagram.com/palingenae/',
          linkClass: 'link_block link__branded--instagram',
          icon: 'fab fa-instagram',
          label: 'Instagram',
        },
        {
          href: 'https://www.github.com/palingenae/',
          linkClass: 'link_block link__branded--github',
          icon: 'fab fa-github',
          label: 'Instagram',
        },
      ],
    }
  },
}
</script>
