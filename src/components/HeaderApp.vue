<template>
  <header>
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
      <!-- <div class="jumbotron-overlay"> -->
      <!-- </div> -->
      <div class="container nav-bar">
        <!-- todo logo -->
        <div class="logo">
          <p>N E X G E N</p>
        </div>

        <nav>
          <ul>
            <li v-for="(link, index) in listLink" :key="index">{{ link }}</li>
            <li><i class="far fa-user"></i></li>
            <li>
              <div class="buttons button-login">get in touch</div>
            </li>
          </ul>
        </nav>
      </div>

      <div class="container">
        <div class="content-jumbo">
          <p class="font-mini-title">logistics services</p>
          <h1>CARGO TRANSPORT</h1>
          <p>
            Fractional or exclusive road cargo transportation to all regions
            with small, medium and large vehicles.
          </p>
          <div class="box-info">
            <div class="buttons button-login">get in touch</div>
            <div class="buttons button-transparent">read more</div>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      listLink: ["Home", "about", "services", "process", "testimonials"],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/header.scss";
</style>