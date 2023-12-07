<script>
export default {
  name: 'Menu',
  data() {
    return {
      menu: [
        {
          nome: 'Characters',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Comics',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Movies',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Tv',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Games',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Collectibles',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Videos',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Fans',
          link: '#',
          target: '_self',
        },
        {
          nome: 'News',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Shop',
          link: '#',
          target: '_self',
        },
      ],
    };
  },
};
</script>
<template>
  <ul class="menu">
    <li v-for="li in menu" class="menu-link">{{ li.nome }}</li>
  </ul>
</template>
<style scoped lang="scss">
// Import
@use '../styles/partials/variables.scss' as *;
@use '../styles/general.scss' as *;

// Stili

.menu {
  display: flex;
  text-transform: uppercase;
  .menu-link {
    margin: 0 15px;
    font-size: 15px;
    font-weight: 500;
    cursor: pointer;
    position: relative;
    text-decoration: none;
    transition: color 0.3s;

    &:hover {
      color: $primary;
    }

    &::after {
      content: '';
      position: absolute;
      bottom: -56px;
      left: 0;
      width: 0%;
      height: 5px;
      background-color: $primary;
      transition: width 0.3s;
    }

    &:hover::after {
      width: 100%;
    }
  }
}
</style>
