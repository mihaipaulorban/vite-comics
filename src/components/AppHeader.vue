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
    <div>
      <Menu />
    </div>
  </header>
</template>
<style scoped></style>
