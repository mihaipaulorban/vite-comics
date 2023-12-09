<script>
export default {
  name: 'ShopSection',
  data() {
    return {
      shopIcons: [
        {
          img: '../../public/img/buy-comics-digital-comics.png',
          name: 'Digital Comics',
          link: '#',
        },
        {
          img: '../../public/img/buy-comics-merchandise.png',
          name: 'DC Merchandise',
          link: '#',
        },
        {
          img: '../../public/img/buy-comics-subscriptions.png',
          name: 'Subscription',
          link: '#',
        },
        {
          img: '../../public/img/buy-comics-shop-locator.png',
          name: 'Comic Shop Locator',
          link: '#',
        },
        {
          img: '../../public/img/buy-dc-power-visa.svg',
          name: 'Dc Power Visa',
          link: '#',
        },
      ],
    };
  },
};
</script>

<template>
  <section class="shop-container">
    <div v-for="icon in shopIcons" :key="icon.name" class="shop-item">
      <img :src="icon.img" :alt="icon.name" />
      <div>{{ icon.name }}</div>
    </div>
  </section>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables.scss' as *;

.shop-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: flex-start;
  align-content: flex-start;
  background-color: $primary;
  overflow: auto;
  flex-direction: row;
  padding: 30px 300px;
  .shop-item {
    display: flex;
    align-items: center;
    flex-direction: row;
    cursor: pointer;
    transition: all 0.2s;

    img {
      max-width: 60px;
      height: 60px;
      object-fit: contain;
    }
    div {
      margin: 5px;
      color: white;
      text-transform: uppercase;
      font-weight: 300;
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
      font-size: 18px;
      margin-left: 15px;
    }

    &:hover {
      color: black;
      filter: invert(1);
    }
  }
}
</style>
