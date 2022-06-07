<template>
  <div class="start">
    <div class="container">
      <div class="start-wrapper">
        <div class="start-block">
          <StartCard />
        </div>
        <div class="start-wrapper-item">
          <div class="start-wrapper-block">
            <div class="start-wrapper__image">
              <img src="@/assets/img/plus.png" alt="" />
            </div>
            <div class="start-block__title">Create an account</div>
          </div>
          <div class="start-wrapper-block">
            <div class="start-wrapper__image">
              <img src="@/assets/img/home.png" alt="" />
            </div>
            <div class="start-block__title">Create an account</div>
          </div>
          <div class="start-wrapper-block">
            <div class="start-wrapper__image">
              <img src="@/assets/img/dollar.png" alt="" />
            </div>
            <div class="start-block__title">Create an account</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import StartCard from "@/components/StartCard";
export default {
  name: "Start",
  components: {
    StartCard,
  },
};
</script>

<style lang="scss" scoped>
.start {
  padding: 50px 0px;
}
.start-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  gap: 50px;
}
.start-wrapper-item {
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.start-wrapper__image img {
  width: 60%;
}
.start-block__title {
  font-weight: bold;
}
@media screen and (max-width: 768px) {
  .start-wrapper__image img {
    width: 40%;
  }
}
@media screen and (max-width: 576px) {
  .start-wrapper-item {
    flex-direction: column;
    gap: 30px;
  }
}
</style>
