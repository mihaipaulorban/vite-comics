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
    <div class="series-banner">CURRENT SERIES</div>
    <MainProducts />
  </main>
</template>
<style scoped lang="scss">
@use '../styles/partials/variables.scss' as *;
@use '../styles/general.scss' as *;
@use '../styles/partials/mixins.scss' as *;

main {
  background-color: $secondary;

  .main-jumbo {
    @include bgImg(
      '../public/img/jumbotron.jpg',
      'no-repeat',
      'center',
      'cover'
    );
    height: 400px;
  }

  .series-banner {
    background-color: $primary;
    color: white;
    font-size: 2rem;
    text-align: center;
    padding: 10px 0;
    font-weight: bold;
    margin-bottom: 20px;
  }
}
</style>
