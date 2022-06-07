<template>
  <div class="start-wrapper-card">
    <div class="start-wrapper__title">Get started in a few minutes</div>
    <div class="start-wrapper__subtitle">
      Coinbase supports a variety of the most popular digital currencies.
    </div>
  </div>
</template>

<script>
export default {
  name: "start-card",
};
</script>
<style scoped lang="scss">
.start-wrapper-card {
  display: flex;
  flex-direction: column;
  gap: 10px;
  .start-wrapper__title {
    font-weight: bold;
    font-size: 30px;
  }
  .start-wrapper__subtitle {
    color: rgba(0, 0, 0, 0.6);
    font-size: 15px;
    font-weight: bold;
  }
}
@media screen and (max-width: 576px) {
  .start-wrapper-card {
    display: flex;
    flex-direction: column;
    .start-wrapper__title {
      font-size: 24px;
    }
    .start-wrapper__subtitle {
      font-size: 13px;
    }
  }
}
</style>
