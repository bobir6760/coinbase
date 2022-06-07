<template>
  <div class="platform-item">
    <div class="platform-info__title">
      The most trusted cryptocurrency platform
    </div>
    <div class="platform-info__subtitle">
      Here are a few reasons why you should choose Coinbase
    </div>
  </div>
</template>

<script>
export default {
  name: "platform-card",
};
</script>
<style lang="scss" scoped>
.platform-info__title {
  font-weight: bold;
  font-size: 30px;
}
.platform-info__subtitle {
  font-size: 20px;
  color: rgba(0, 0, 0, 0.4);
}
@media screen and (max-width: 992px) {
  .platform-info__title {
    font-size: 25px;
  }
  .platform-info__subtitle {
    font-size: 17px;
  }
}
@media screen and (max-width: 769px) {
  .platform-info__title {
    font-size: 23px;
  }
  .platform-info__subtitle {
    font-size: 15px;
  }
}
</style>
