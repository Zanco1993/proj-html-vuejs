<template>
  <div class="container">
    <a name="info"></a>
    <div class="get-in-touch">
      <div class="info-user">
        <p class="font-mini-title color"><strong>send a message</strong></p>
        <div class="title">
          <span class="font-title">Get in</span>
          <span class="bg-title font-title">Touch</span>
        </div>
        <div class="description-service">
          <p class="info-service">
            We will respond to your message as soon as possible.
          </p>
        </div>

        <div class="box-input">
          <input type="text" placeholder="Name" />
          <input type="email" placeholder="Email" />
          <input type="text" placeholder="Phone" />
          <input type="text" placeholder="More info" />
        </div>
        <textarea rows="8" placeholder="Message"></textarea>
        <span class="buttons button-login">Send</span>
      </div>

      <div class="contact">
        <h3>Example Inc.</h3>
        <p class="py-4">
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Harum,
          commodi?
        </p>
        <p class="py-4">
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Harum,
          commodi?
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
          <span class="buttons button-transparent">view map</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../style/getInTouch.scss";
</style>