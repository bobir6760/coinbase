<template>
  <div class="create-info">
    <div class="create-info__title">
      Create your cryptocurrency portfolio today
    </div>
    <div class="create-info__subtitle">
      Coinbase has a variety of features that make it the best place to start
      trading
    </div>
  </div>
</template>

<script>
export default {
  name: "create-card",
};
</script>
<style scoped lang="scss">
.create-info {
  display: flex;
  flex-direction: column;
  text-align: center;
  gap: 20px;
  .create-info__title {
    font-size: 35px;
    font-weight: bold;
  }
  .create-info__subtitle {
    font-size: 18px;
    color: gray;
  }
}
</style>
