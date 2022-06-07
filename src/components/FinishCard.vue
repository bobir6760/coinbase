<template>
  <div class="finish-wrapper-card">
    <div class="finish-wrapper__title">Earn up to $7 worth of <br />crypto</div>
    <div class="finish-wrapper__subtitle">
      Discover how specific cryptocurrencies work — and <br />get a bit of each
      crypto to try out for yourself.
    </div>
    <div class="finish-wrapper__btn">
      <button class="finish-btn">Start earning</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "finish-card",
};
</script>
<style lang="scss" scoped>
.finish-wrapper-card {
  display: flex;
  flex-direction: column;
  gap: 10px;
  .finish-wrapper__title {
    font-size: 50px;
  }
  .finish-wrapper__subtitle {
    font-size: 20px;
  }
  .finish-btn {
    cursor: pointer;
    color: #fff;
    background: #0075ff;
    border-radius: 5px;
    border: none;
    padding: 12px 30px;
  }
  .finish-btn:active {
    color: black;
  }
}
@media screen and (max-width: 1200px) {
  .finish-wrapper-card {
    display: flex;
    flex-direction: column;
    gap: 10px;
    .finish-wrapper__title {
      font-size: 35px;
    }
    .finish-wrapper__subtitle {
      font-size: 15px;
    }
    .finish-btn {
      cursor: pointer;
      color: #fff;
      background: #0075ff;
      border-radius: 5px;
      border: none;
      padding: 10px 25px;
    }
  }
}
@media screen and (max-width: 992px) {
  .finish-wrapper-card {
    display: flex;
    flex-direction: column;
    gap: 10px;
    .finish-wrapper__title {
      font-size: 35px;
    }
    .finish-wrapper__subtitle {
      font-size: 11px;
    }
    .finish-btn {
      cursor: pointer;
      color: #fff;
      background: #0075ff;
      border-radius: 5px;
      border: none;
      padding: 10px 25px;
    }
  }
}
@media screen and (max-width: 769px) {
  .finish-wrapper-card {
    .finish-wrapper__title {
      font-size: 20px;
    }
    .finish-wrapper__subtitle {
      font-size: 15px;
    }
    .finish-btn {
      padding: 6px 20px;
      font-size: 11px;
    }
  }
}
@media screen and (max-width: 576px) {
  .finish-wrapper-card {
    .finish-wrapper__title {
      font-size: 25px;
    }
    .finish-wrapper__subtitle {
      font-size: 13px;
    }
  }
}
</style>
