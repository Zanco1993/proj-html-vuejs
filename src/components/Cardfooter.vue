<template>
  <div class="card bg-card">
    <h1 class="py-4">{{ link.title }}</h1>
    <ul>
      <li v-for="info in link.info" :key="info">
        <i class="fas fa-chevron-right"></i>
        <span>{{ info }}</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    link: Object,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variablesColor.scss";

.bg-card {
  background-color: $Shark;
  padding: 20px 30px;

  h1 {
    color: $White;
  }
  ul {
    list-style: none;

    li {
      margin-bottom: 10px;

      span {
        padding-left: 10px;
      }
    }
  }
}
</style>