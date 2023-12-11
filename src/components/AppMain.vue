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
    background-size: cover;

    height: 400px;
  }
}
</style>
