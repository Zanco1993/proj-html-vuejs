<template>
  <div class="bg">
    <a name="process"></a>
    <div class="logistical text-center">
      <div class="info-stories">
        <p class="font-mini-title color-title">
          <strong>how it works in practice</strong>
        </p>

        <span class="bg-title font-title">Logistical</span>
        <span class="font-title">Procedure</span>

        <p>
          We work with innovative methodologies to ensure that the entire
          delivery process is done from start to finish as planned.
        </p>
      </div>
    </div>

    <div class="process">
      <card-logistic v-for="(process, index) in processInfo" :key="index" :process="process" />
      
    </div>
  </div>
</template>

<script>
import CardLogistic from "./CardLogistic.vue";
export default {
  data() {
    return {
      processInfo: [
        {
          title: "Collection of information",
          text: "Lorem ipsum dolor sit amet consectetur.",
          numberProcess: "01",
        },
        {
          title: "Service Invoice Sending",
          text: "Lorem ipsum dolor sit amet consectetur.",
          numberProcess: "02",
        },
        {
          title: "Withdrawal of Cargo",
          text: "Lorem ipsum dolor sit amet consectetur.",
          numberProcess: "03",
        },
        {
          title: "Transport Customer Order",
          text: "Lorem ipsum dolor sit amet consectetur.",
          numberProcess: "04",
        },
        {
          title: "Successful Delivery",
          text: "Lorem ipsum dolor sit amet consectetur.",
          numberProcess: "05",
        },
      ],
    };
  },
  components: {
    CardLogistic,
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/logistical.scss";
</style>