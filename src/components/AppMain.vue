<script>
import MainProducts from './MainProducts.vue';
export default {
  name: 'main',
  components: {
    MainProducts,
  },
};
</script>
<template>
  <main>
    <div class="main-jumbo"></div>
    <div class="content-container">
      <div class="series-banner">CURRENT SERIES</div>
      <MainProducts />
    </div>
    <button class="load-more-btn">LOAD MORE</button>
  </main>
</template>
<style scoped lang="scss">
@use '../styles/partials/variables.scss' as *;
@use '../styles/general.scss' as *;
@use '../styles/partials/mixins.scss' as *;

main {
  background-color: $secondary;
  padding-bottom: 30px;

  .main-jumbo {
    @include bgImg(
      '../public/img/jumbotron.jpg',
      'no-repeat',
      'center',
      'cover'
    );
    height: 400px;
  }

  .content-container {
    position: relative;
  }

  .series-banner {
    background-color: $primary;
    color: white;
    font-size: 1.7rem;
    padding: 10px 20px;
    font-weight: bold;
    position: absolute;
    top: -20px;
    left: 200px;
  }
  .load-more-btn {
    background-color: $primary;
    color: white;
    padding: 15px 40px;
    margin: 0 auto;
    display: block;
    font-size: 0.8rem;
    border: none;
    cursor: pointer;
    transition: background-color 0.2s ease;

    &:hover {
      background-color: white;
      color: $primary;
    }
  }
}
</style>
