<template>
  <div class="logo">
    <span class="decoration">N E X </span>
    <span>G E N</span>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>

@import "@/style/variablesColor.scss";

.logo {
  span {
    font-weight: 900;
  }

  .decoration {
    padding-left: 25px;
    padding-top: 10px;
    padding-bottom: 10px;
    border-top-left-radius: 20px;
    border-bottom-left-radius: 20px;
    background-color: #0e272dc9;
    color: $FountainBlue;
  }
}
</style>