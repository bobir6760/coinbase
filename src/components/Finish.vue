<template>
  <div class="finish">
    <div class="container">
      <div class="finish-wrapper">
        <div class="finish-wrapper-item">
          <FinishCard />
        </div>
        <div class="finish-image">
          <img src="@/assets/img/big.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import FinishCard from "@/components/FinishCard";
export default {
  name: "Finish",
  components: {
    FinishCard,
  },
};
</script>

<style lang="scss" scoped>
.finish {
  padding: 50px 0px;
  background: #f5f8ff;
}
.finish-wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.finish-image {
  text-align: end;
  border-radius: 20px;
  overflow: hidden;
}
.finish-image img {
  width: 80%;
}
@media screen and (max-width: 769px) {
  .finish-image img {
    width: 75%;
  }
}
@media screen and (max-width: 576px) {
  .finish-wrapper {
    flex-direction: column;
    gap: 30px;
    text-align: center;
  }
}
</style>
