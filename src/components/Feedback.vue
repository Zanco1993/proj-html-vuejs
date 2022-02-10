<template>
  <div class="bg">
    <a name="testimonials"></a>
    <div class="service">
      <div class="container">
        <p class="font-mini-title text-center">
          <strong>customer testimonials</strong>
        </p>
        <div class="title text-center">
          <span class="font-title">Trusted</span>
          <span class="bg-title font-title">Feedback</span>
        </div>

        <p class="info-service text-center">
          We work intensively in search of ideals that can add up in the lives
          of our customers. This is what moves us and we are grateful for the
          recognition.
        </p>

        <div class="box-card">
          <card-feedback
            v-for="(feed, index) in listFeedback"
            :key="index"
            :feed="feed"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CardFeedback from "./CardFeedback.vue";
export default {
  data() {
    return {
      listFeedback: [
        {
          image: "logo-1.png",
          firstText:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. In soluta pariatur aliquid quaerat libero perspiciatis magni delectus ut unde omnis beatae, voluptatem expedita deleniti.",
          secondText:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. In soluta pariatur aliquid.",
        },
        {
          image: "logo-2.png",
          firstText:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. In soluta pariatur aliquid quaerat libero perspiciatis magni delectus ut unde omnis beatae, voluptatem expedita deleniti.",
          secondText:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. In soluta pariatur aliquid.",
        },
        {
          image: "logo-3.png",
          firstText:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. In soluta pariatur aliquid quaerat libero perspiciatis magni delectus ut unde omnis beatae, voluptatem expedita deleniti.",
          secondText:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. In soluta pariatur aliquid.",
        },
      ],
    };
  },
  components: {
    CardFeedback,
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/feedback.scss";
</style>