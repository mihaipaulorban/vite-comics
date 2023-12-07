<script>
export default {
  name: 'main',
};
</script>
<template>
  <main>
    <div class="content">Content Goes Here</div>
  </main>
</template>
<style scoped lang="scss">
@use '../styles/partials/variables.scss' as *;
@use '../styles/general.scss' as *;

main {
  background-color: $secondary;
  color: white;
  padding: 50px;
  font-size: 40px;
}
</style>
