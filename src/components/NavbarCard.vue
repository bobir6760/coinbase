<template>
  <div class="navbar-info">
    <div class="navbar-wrapper__title">
      <p>Prices</p>
      <p>Learn</p>
      <p>Individuals</p>
      <p>Businesses</p>
      <p>Developers</p>
      <p>Company</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "navbar-card",
};
</script>

<style scoped lang="scss">
.navbar-info {
  display: flex;
  .navbar-wrapper__title {
    display: flex;
    gap: 30px;
    font-size: 20px;
  }
}
@media screen and (max-width: 1200px) {
  .navbar-info .navbar-wrapper__title {
    font-size: 15px;
    gap: 15px;
  }
}
@media screen and (max-width: 992px) {
  .navbar-info .navbar-wrapper__title {
    font-size: 12px;
    gap: 10px;
  }
}
@media screen and (max-width: 576px) {
  .navbar-info .navbar-wrapper__title {
    font-size: 11px;
    gap: 10px;
  }
}
</style>
