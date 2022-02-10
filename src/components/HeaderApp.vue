<template>
  <header>
    <a name="home"></a>
    <div class="content-info">
      <div class="container contacts">
        <div class="open-hours">
          <i class="fas fa-clock"></i>
          <span> Open Hours: Mon - Sat - 9:00 - 18:00</span>
        </div>
        <div class="info-social">
          <ul>
            <li>
              <i class="fas fa-phone"></i>
              <span> +1 (305) 1234-5678</span>
            </li>
            <li>
              <i class="fas fa-envelope"></i>
              <span> hello@example.com</span>
            </li>
            <li><i class="fab fa-facebook-f"></i></li>
            <li><i class="fab fa-twitter"></i></li>
            <li><i class="fab fa-linkedin-in"></i></li>
          </ul>
        </div>
      </div>
    </div>

    <div class="jumbotron">
      <div class="jumbotron-overlay"></div>
      <div class="container nav-bar on-overlay">
        <logo-app />

        <nav>
          <ul>
            <li v-for="(link, index) in listLink" :key="index">
              <a :href="`#${link.title}`">{{ link.url }}</a>
            </li>
            <li><i class="far fa-user"></i></li>
            <li>
              <a href="#info" class="buttons button-login">get in touch</a>
            </li>
          </ul>
          
        </nav>
      </div>

      <div class="container on-overlay">
        <div class="content-jumbo">
          <p class="font-mini-title py-4">logistics services</p>
          <h1>CARGO TRANSPORT</h1>
          <p class="py-4">
            Fractional or exclusive road cargo transportation to all regions
            with small, medium and large vehicles.
          </p>
          <div class="box-info py-4">
            <div class="buttons button-login mr-4">get in touch</div>
            <div class="buttons button-transparent">read more</div>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import LogoApp from "./logoApp.vue";
export default {
  components: {
    LogoApp,
  },
  data() {
    return {
      listLink: [
        {
          title: "home",
          url: "home",
        },
        {
          title: "about",
          url: "about",
        },
        {
          title: "services",
          url: "services",
        },
        {
          title: "process",
          url: "process",
        },
        {
          title: "testimonials",
          url: "testimonials",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/header.scss";
</style>