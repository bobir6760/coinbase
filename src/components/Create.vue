<template>
  <div class="create">
    <div class="container">
      <div class="create-wrapper">
        <div class="crate-card-wrapper">
          <CreateCard />
        </div>
        <div class="create-wrapper-card">
          <div class="create-wrappet-body">
            <div class="create-card-block">
              <div class="create-card__image">
                <img src="@/assets/img/Vector1.svg" alt="" />
              </div>
              <div class="create-card-item">
                <div class="create-card__title">Manage your portfolio</div>
                <div class="create-card__subtitle">
                  Buy and sell popular digital currencies, <br />keep track of
                  them in the one place.
                </div>
              </div>
            </div>
            <div class="create-card-block">
              <div class="create-card__image">
                <img src="@/assets/img/Vector2.svg" alt="" />
              </div>
              <div class="create-card-item">
                <div class="create-card__title">Manage your portfolio</div>
                <div class="create-card__subtitle">
                  Buy and sell popular digital currencies, <br />keep track of
                  them in the one place.
                </div>
              </div>
            </div>
            <div class="create-card-block">
              <div class="create-card__image">
                <img src="@/assets/img/Vector3.svg" alt="" />
              </div>
              <div class="create-card-item">
                <div class="create-card__title">Manage your portfolio</div>
                <div class="create-card__subtitle">
                  Buy and sell popular digital currencies, <br />keep track of
                  them in the one place.
                </div>
              </div>
            </div>
          </div>
          <div class="create-wrapper__image">
            <img src="@/assets/img/Chart.png" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CreateCard from "@/components/CreateCard";
export default {
  name: "Create",
  components: {
    CreateCard,
  },
};
</script>

<style scoped lang="scss">
.create {
  padding: 50px 0px;
}
.create-wrapper {
  display: flex;
  flex-direction: column;
  text-align: center;
  gap: 50px;
}
.create-wrappet-body {
  display: flex;
  flex-direction: column;
  gap: 30px;
  .create-card-block {
    display: flex;
    gap: 20px;
    align-items: center;
    .create-card__image img {
      width: 100%;
    }
    .create-card__image {
      border-radius: 30px;
      background: #ffffff;
      box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
      padding: 8px 9px 5px 10px;
    }
  }
  .create-card-item {
    display: flex;
    flex-direction: column;
    gap: 15px;
    .create-card__title {
      font-size: 22px;
      font-weight: bold;
    }
    .create-card__subtitle {
      font-size: 18px;
      color: gray;
    }
  }
}
.create-wrapper-card {
  display: flex;
  justify-content: center;
  gap: 50px;
}
.create-wrapper__image img {
  width: 100%;
}
@media screen and (max-width: 992px) {
  .create-wrappet-body .create-card-item {
    display: flex;
    flex-direction: column;
    gap: 10px;
    .create-card__title {
      font-size: 18px;
      font-weight: bold;
    }
    .create-card__subtitle {
      font-size: 10px;
      color: gray;
    }
  }
  .create-wrappet-body .create-card-block {
    .create-card__image img {
      width: 80%;
    }
    .create-card__image {
      border-radius: 30px;
      background: #ffffff;
      box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
      padding: 6px 6px 2px 10px;
    }
  }
}
@media screen and (max-width: 768px) {
  .create-wrappet-body .create-card-item {
    display: flex;
    flex-direction: column;
    gap: 10px;
    .create-card__title {
      font-size: 15px;
      font-weight: bold;
    }
    .create-card__subtitle {
      font-size: 6px;
      color: gray;
    }
  }
  .create-info {
    display: flex;
    flex-direction: column;
    text-align: center;
    gap: 20px;
    .create-info__title {
      font-size: 25px;
      font-weight: bold;
    }
    .create-info__subtitle {
      font-size: 13px;
      color: gray;
    }
  }
}
@media screen and (max-width: 576px) {
  .create-wrapper-card {
    display: flex;
    flex-direction: column;
    gap: 50px;
  }
  .create-wrappet-body .create-card-block {
    justify-content: center;
  }
}
</style>
