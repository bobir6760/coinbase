<template>
  <div class="platform-wrapper__item">
    <div class="platform-block__image">
      <img :src="item.imgUrl" alt="" />
    </div>
    <div class="platform-block__title">{{ item.title }}</div>
    <div class="platform-block__subtitle">{{ item.subtitle }}</div>
  </div>
</template>
<script>
export default {
  name: "platform-body",
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
};
</script>
<style lang="scss" scoped>
.platform-wrapper__item {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;
  .platform-wrapper__block {
    display: flex;
    gap: 10px;
    .platform-block__image img {
      width: 100%;
    }
  }
  .platform-block__title {
    font-size: 23px;
    font-weight: bold;
  }
  .platform-block__subtitle {
    color: rgba(0, 0, 0, 0.6);
    font-size: 20px;
  }
}
</style>
