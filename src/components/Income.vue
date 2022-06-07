<template>
  <div class="income">
    <div class="container">
      <div class="income-wrapper">
        <div class="income-wrapper-item">
          <div class="income-wrapper__title">$547B</div>
          <div class="income-wrapper__subtitle">Quarterly volume traded</div>
        </div>
        <div class="income-wrapper-item">
          <div class="income-wrapper__title">100+</div>
          <div class="income-wrapper__subtitle">Countries supported</div>
        </div>
        <div class="income-wrapper-item">
          <div class="income-wrapper__title">89+M</div>
          <div class="income-wrapper__subtitle">Verified users</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Income",
};
</script>

<style lang="scss" scoped>
.income {
  padding: 50px 0px;
  background: #0075ff;
}
.income-wrapper {
  display: flex;
  justify-content: space-around;
  text-align: center;
  align-items: center;
  .income-wrapper-item {
    display: flex;
    flex-direction: column;
    gap: 5px;
    .income-wrapper__title {
      font-size: 50px;
      color: #fff;
    }
    .income-wrapper__subtitle {
      color: rgba(255, 255, 255, 0.6);
      font-size: 15px;
    }
  }
}
@media screen and (max-width: 768px) {
  .income-wrapper .income-wrapper-item .income-wrapper__title {
    font-size: 35px;
  }
  .income-wrapper .income-wrapper-item .income-wrapper__subtitle {
    font-size: 12px;
  }
}
@media screen and (max-width: 576px) {
  .income-wrapper {
    display: flex;
    flex-direction: column;
    gap: 30px;
  }
}
</style>
