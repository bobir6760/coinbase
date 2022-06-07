<template>
  <div class="platform">
    <div class="container">
      <div class="platform-wrapper">
        <div class="platform-card-wrapper">
          <PlatformCard />
        </div>
        <div class="platform-wrapper-card">
          <PlatformBody
            v-for="(card, index) in cards"
            :key="index"
            :item="card"
          />
        </div>
        <div class="platyform-card">
          <div class="platform-card-block">
            <div class="platform-card__title">
              Learn how Coinbase keeps your funds <br />safe and secure
            </div>
            <div class="platform-card__title">
              Learn how Coinbase keeps your funds <br />safe and secure
            </div>
            <div class="platform-card__title">
              Learn how Coinbase keeps your funds <br />safe and secure
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import PlatformCard from "@/components/PlatformCard";
import PlatformBody from "@/components/PlatformBody";
export default {
  name: "Platform",
  data() {
    return {
      cards: [
        {
          imgUrl: require("@/assets/img/walp1.png"),
          title: "Secure storage",
          subtitle:
            "We store the vast majority of the digital assets in secure offline storage.",
        },
        {
          imgUrl: require("@/assets/img/walp2.png"),
          title: "Secure storage",
          subtitle:
            "We store the vast majority of the digital assets in secure offline storage.",
        },
        {
          imgUrl: require("@/assets/img/walp3.png"),
          title: "Secure storage",
          subtitle:
            "We store the vast majority of the digital assets in secure offline storage.",
        },
      ],
    };
  },
  components: {
    PlatformCard,
    PlatformBody,
  },
};
</script>

<style lang="scss" scoped>
.platform {
  padding: 50px 0px;
}
.platform-wrapper {
  display: flex;
  flex-direction: column;
  gap: 50px;
  text-align: center;
}
.platform-item {
  display: flex;
  flex-direction: column;
  gap: 10px;
}
.platform-wrapper-card {
  display: flex;
  gap: 20px;
}
.platform-card-block {
  display: flex;
  justify-content: center;
  gap: 70px;
  .platform-card__title {
    color: #0075ff;
    font-size: 20px;
  }
}
@media screen and (max-width: 1200px) {
  .platform-wrapper__item .platform-block__subtitle {
    font-size: 15px;
  }
  .platform-card-block {
    gap: 50px;
  }
  .platform-card-block .platform-card__title {
    font-size: 15px;
  }
}
@media screen and (max-width: 992px) {
  .platform-wrapper__item .platform-block__subtitle {
    font-size: 12px;
  }
  .platform-wrapper__item .platform-block__title {
    font-size: 15px;
  }
  .platform-card-block {
    gap: 20px;
  }
  .platform-card-block .platform-card__title {
    font-size: 11px;
  }
}
@media screen and (max-width: 768px) {
  .platform-wrapper__item .platform-block__subtitle {
    font-size: 10px;
  }
  .platform-wrapper__item .platform-block__title {
    font-size: 15px;
  }
  .platform-card-block {
    gap: 20px;
  }
}
@media screen and (max-width: 576px) {
  .platform-wrapper__item {
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  .platform-wrapper__item .platform-block__subtitle {
    font-size: 15px;
  }
  .platform-wrapper__item .platform-block__title {
    font-size: 20px;
  }
  .platform-card-block {
    display: flex;
    flex-direction: column;
    gap: 15px;
  }
  .platform-card-block .platform-card__title {
    font-size: 16px;
  }
  .platform-wrapper-card {
    flex-direction: column;
  }
}
</style>
