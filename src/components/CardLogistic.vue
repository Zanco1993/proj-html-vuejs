<template>
  <div class="card-info">
    <h3>{{process.title}}</h3>
    <p>{{process.text}}</p>
    <span class="number-process"> {{process.numberProcess}} </span>
  </div>
</template>
<script>
export default {
    props: {
        process: Object
    }
};
</script>

<style lang="scss" scoped>
@import "@/style/variablesColor.scss";
.card-info {
  width: calc(100% / 5);
  text-align: center;
  position: relative;
  color: $MidGray;

  h3 {
    padding: 30px 40px;
    color: #000;
  }
  p {
    color: $MidGray;
  }

  .number-process {
    position: absolute;
    top: 0;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #daeced;
    color: $BluChill;
    padding: 10px;
    border-radius: 50%;
    font-weight: bold;
  }
}
</style>