<script>
import Menu from './Menu.vue';
export default {
  name: 'Header',

  components: {
    Menu,
  },
};
</script>
<template>
  <header>
    <div class="content-container">
      <img src="../../public/img/dc-logo.png" alt="" />
      <Menu />
    </div>
  </header>
</template>
<style scoped lang="scss">
.content-container {
  padding: 20px 300px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

img {
  width: 90px;
}
</style>
