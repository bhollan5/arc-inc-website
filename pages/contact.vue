<template>
  <section>
    <div id="contact-background">
      <div class="dark-text-box">
        <h1>Contact Us</h1>
        <p>Contact us through phone or email for pricing.</p>
        <br>
        <p class="contact-line">
          <img src="@/assets/icons/mail.png" width="25" style="margin-right:10px;">
          <a href="mailto:tgresock@hollandmgmt.com">
            tgresock@hollandmgmt.com
          </a>
        </p>
        <p class="contact-line">
          <img src="@/assets/icons/phone.png" width="25" style="margin-right:10px;">
          <a href="tel:555-555-5555">555-555-5555</a>
        </p>
      </div>
    </div>
    
  </section>
</template>

<script>

export default {
  name: 'contact',
  data() {
    return {
    }
  }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/variables';

#contact-background {
  padding-top: 200px;
  height: 200vh;
  background: url('../assets/contact_bg.png');
  background-size: cover;
}

.dark-text-box {
  background: rgba(0,0,0,.8);
  width: 90%;
  max-width: 700px;
  min-height: 100px;
  margin-left: 50%;
  padding: 20px;
  transform: translatex(-50%);
  text-align: center;
  color: white;
  font-size: 18px;
  h1 {
    font-size: 30px;
    font-weight: bold;
  }
}

.contact-line {
  display: flex;
  align-items: center;
  width: 30%;
  margin-left: 35%;
  text-decoration: underline;
  justify-content: space-between;
  margin-bottom: 20px;
  a {
    color: white;
  }
  @media only screen and (max-width: $bp) {
    margin-left: 0px;
    width: 100%;
  }
}

</style>
