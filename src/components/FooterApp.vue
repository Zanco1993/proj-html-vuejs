<template>
  <div>
    <footer>
      <div class="container box-card">
        <div class="card">
          <logo-app />
          <p class="py-4">
            A functional HTML Template for Corporate & Business
          </p>

          <div class="generic-info">
            <i class="fas fa-phone"></i>
            <span> +1 (305) 1234-5678</span>
          </div>
          <div class="generic-info">
            <i class="fas fa-envelope"></i>
            <span>hello@example.com</span>
          </div>
          <div class="generic-info">
            <i class="fas fa-map-marker-alt"></i>
            <span>Main Avenue, 987</span>
          </div>
          <div class="generic-info">
            <span class="buttons button-transparent">get in touch</span>
          </div>
        </div>

        <cardfooter
          v-for="(link, index) in linkFooter"
          :key="index"
          :link="link"
        />
      </div>

      <div class="credits">
        <div class="container policy">
          <p>Enjoy the low price. We are tracking any intention of privacy</p>
          <p>
            <i class="far fa-copyright"></i> 2020 NEXGEN is Proudly Powered by
            <span>Codings</span>.
          </p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import Cardfooter from "./Cardfooter.vue";
import LogoApp from "./logoApp.vue";
export default {
  data() {
    return {
      linkFooter: [
        {
          title: "About",
          info: [
            "The Company",
            "Institutional",
            "Social & Events",
            "Innovation",
            "Environment",
            "Technology",
          ],
        },
        {
          title: "Transport",
          info: [
            "Industrialized",
            "Chemicals",
            "Packaged Liquids",
            "Construction",
            "Laminated Wood",
            "And others",
          ],
        },
        {
          title: "Support",
          info: [
            "Responsability",
            "Terms of Use",
            "About Cookies",
            "Privacy Policy",
            "Accessibily",
            "Information",
          ],
        },
      ],
    };
  },
  components: {
    Cardfooter,
    LogoApp,
  },
};
</script>

<style lang="scss" scoped>
@import "../style/footer.scss";
</style>