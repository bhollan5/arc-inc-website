<template>
  <section>
    <div class="image-banner">
      <img src="../../assets/senior_living/services_banner.png">
      <div id="banner-text">
        <h1>What We Do</h1>
        <p>As senior community owners ourselves, we are experts in the unique characteristics of senior living design. </p>
      </div>
      
    </div>
    <div id="services">
      <h2>ARC Senior Living Services</h2>
      <ul>
        <li>»	Operational review of spaces.</li>
        <li>»	Space planning.</li>
        <li>»	Selection of finish & materials.</li>
        <li>»	Furniture procurement, maintaining relationships with vendors.</li>
        <li>»	Specification of furniture, accessories, artwork, plants, decorative lighting, & window treatment.</li>
        <li>»	Consultation access for your business' future needs.</li>
        <li>»	Design for renovated spaces as well as new construction.</li>
        <li>»	Construction documents for all interior finishes – flooring, walls, ceiling, art placement.</li>
        <li>»	Provide conceptual images and sketches.</li>
      </ul>
      <button class="blue-action-button">
        Contact us for pricing →
      </button>
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
    
  }
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
#services {
  font-family: CrimsonText;
  padding: 100px;
  color: $navy;
  button {
    margin-left: 50%;
    transform: translatex(-50%);
    margin-top: 50px;
    margin-bottom: 50px;
  }
}
h2 {
  text-align: center;
  font-size: 40px;
  font-weight: bold;
}
ul {
  margin: 50px 20%;
  font-size: 24px;
}
</style>
