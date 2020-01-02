<template>
  <section>
    <div class="image-banner">
      <img src="../../assets/senior_living/services_banner.png">
      <div id="banner-text">
        <h1>What We Do</h1>
        <p>As senior community owners ourselves, we are experts in the unique characteristics of senior living design. </p>
      </div>
      
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
  #banner-text {
    padding-left: 50px; 

    width: 50%;
    min-width: 500px;
    background: rgba(0,0,0,.45);
    height: 100%;
    top: 0px;
    position: absolute;
    right: 0px;
    text-align: left;
    h1 {
      margin: 0px;
      margin-top: 30%;
      transform: none;
    }
    p {
      font-size: 20px;
      width: 60%;
    }
  }
}
</style>
