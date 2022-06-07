<template>
  <div class="best">
    <div class="container">
      <div class="best-wrapper">
        <div class="best-info">
          <div class="best-wrapper__block">
            <div class="best-info__title">Jump start your portfolio</div>
            <div class="best-info__image">
              <img src="@/assets/img/art.svg" alt="" />
            </div>
          </div>
          <div class="best-wrapper-card">
            <div class="best-card__title">
              Jump start <br />your crypto<br />
              portfolio
            </div>
            <div class="best-card__subtitle">
              Coinbase is the easiest place to buy and sell
              <br />cryptocurrency. Sign up and get started today.
            </div>
            <div class="best-block">
              <div class="best-card__input">
                <input placeholder="Email addres" type="text" />
              </div>
              <div class="best-card__btn">
                <button class="best-btn">Get started</button>
              </div>
            </div>
          </div>
        </div>
        <div class="best-card-wrapper">
          <BestCard />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import BestCard from "@/components/BestCard";
export default {
  name: "Best",
  components: {
    BestCard,
  },
};
</script>

<style lang="scss" scoped>
.best {
  padding: 50px 0px;
}
.best-wrapper {
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.best-info {
  display: flex;
  flex-direction: column;
  gap: 10px;
}
.best-wrapper__block {
  display: flex;
  gap: 5px;
  .best-info__title {
    color: #0075ff;
    font-weight: bold;
  }
  .best-info__image img {
    width: 100%;
  }
}

.best-wrapper-card {
  display: flex;
  flex-direction: column;
  gap: 15px;
  .best-card__title {
    font-size: 60px;
    font-weight: bold;
  }
  .best-card__subtitle {
    font-size: 20px;
  }
}
.best-block {
  display: flex;
  gap: 10px;
  .best-card__input input {
    padding: 10px 30px 10px 17px;
    font-size: 18px;
    border-radius: 5px;
    border-color: gray;
    color: rgba(0, 0, 0, 0.4);
  }
  .best-btn {
    cursor: pointer;
    color: white;
    background: #0075ff;
    padding: 12px 40px;
    border-radius: 5px;
    border: none;
    font-size: 18px;
  }
  .best-btn:active {
    color: black;
  }
}
@media screen and (max-width: 992px) {
  .best-wrapper-card {
    display: flex;
    flex-direction: column;
    gap: 15px;
    .best-card__title {
      font-size: 50px;
      font-weight: bold;
    }
    .best-card__subtitle {
      font-size: 15px;
    }
  }
  .best-block {
    display: flex;
    flex-direction: column;
    gap: 10px;
    .best-card__input input {
      padding: 10px 30px 10px 17px;
      font-size: 15px;
    }
    .best-btn {
      padding: 12px 40px;
      font-size: 15px;
    }
  }
}
@media screen and (max-width: 768px) {
  .best-wrapper-card {
    .best-card__title {
      font-size: 40px;
    }
    .best-card__subtitle {
      font-size: 12px;
    }
  }
}
@media screen and (max-width: 576px) {
  .best-wrapper {
    flex-direction: column;
    text-align: center;
    gap: 30px;
  }
}
</style>
