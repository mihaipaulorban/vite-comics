<script>
import DownList from './DownList.vue';
export default {
  name: 'footer',
  components: {
    DownList,
  },
};
</script>
<template>
  <div class="info-section">
    <DownList />
    <img src="../../public/img/dc-logo-bg.png" alt="" />
  </div>
</template>
<style scoped>
.info-section {
  display: flex;
  justify-content: space-between;
  background-image: url(../../public/img/footer-bg.jpg);
  align-items: center;
  overflow: hidden;
  height: 400px;
  padding: 0 300px;

  img {
    width: 600px;
    height: 600px;
  }
}
</style>
