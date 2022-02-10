<template>
  <div class="content-card">
    <div class="box-image">
      <img :src="`/img/${feed.image}`" alt="" />
    </div>

    <p class="py-4">
      {{ feed.firstText }}
    </p>
    <p>
      {{ feed.secondText }}
    </p>
    <i class="fas fa-quote-right icon"></i>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  props: {
    feed: Object,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variablesColor.scss";

.content-card {
  width: 350px;
  height: 300px;
  padding: 30px;
  background-color: $Shark;
  border-radius: 10px;
  position: relative;

  img {
    filter: invert(1);
  }

  .icon {
    position: absolute;
    right: 20px;
    font-size: 30px;
    color: $MidGray;
  }
}
</style>