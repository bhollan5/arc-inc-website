<template>
  <section>
    <div class="image-banner">
      <img src="../../assets/home_staging/photo_a.png">
      <div id="services-banner-text">
        <h1>Home Staging Services</h1>
        <p>We're offering our interior design services to increase the value of your property for sale. </p>
      </div>
      
    </div>
    <div id="services">
      <h2>ARC Home Staging Services </h2>
      <p>Our home staging services include <b>empty home staging </b>for realtors, home owners, and investors.</p>
      <p><b>Any number of rooms can be staged,</b> including but not limited to kitchens, master suites, bathrooms, living rooms, and dining rooms. </p>
      <router-link to="/contact" tag="button" class="blue-action-button">
        Contact us for pricing →
      </router-link>
    </div>
    
  </section>
</template>

<script>

export default {
  name: 'seniorServices',

}
</script>

<style scoped lang="scss">
@import '../../assets/styles/variables';

.image-banner {
  height: 600px;
  @media only screen and (max-width: $bp) {
    height: 300px;
  }
  
  #services-banner-text {
    padding-left: 50px; 

    width: 50%;
    @media only screen and (max-width: $bp) {
      width: 100%;
      padding-left: 10%;
    }
    // min-width: 500px;
    background: rgba(0,0,0,.45);
    height: 100%;
    top: 0px;
    position: absolute;
    right: 0px;
    text-align: left;
    h1 {
      margin: 0px;
      margin-top: 30%;
      @media only screen and (max-width: $bp) {
        margin-top: 10%;
        font-size: 2em;
      }
      transform: none;
    }
    p {
      font-size: 20px;

      width: 60%;
      @media only screen and (max-width: $bp) {
        width: 100%;
      }
    }
  }
}
#services {
  font-family: CrimsonText;
  padding: 100px;
  @media only screen and (max-width: $bp) {
    padding: 10%;
  }
  color: $navy;
  button {
    margin-left: 50%;
    transform: translatex(-50%);
    margin-top: 50px;
    margin-bottom: 50px;
    min-width: 100px;
    display: block;
  }
  p {
    text-align: center;
    font-size: 20px;
    margin: 25px ;
  }
}
h2 {
  text-align: center;
  font-size: 40px;
  font-weight: bold;
}
ul {
  margin: 50px 20%;
  @media only screen and (max-width: $bp) {
    margin: 50px 0%;
  }
  font-size: 24px;
}
</style>
