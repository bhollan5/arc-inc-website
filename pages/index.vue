<template>
  <section>



    <!-- The landing page -->
    <div id="option-banners">

      <!-- Senior living section -->
      <div id="senior-living-banner" class="banner-section">
        <div class="banner-image" id="senior-living-image"></div>
        <h2>Senior Living</h2>
        <p>For decades, ARC Inc. has been designing thoughtful, dignified spaces for the senior living community. </p>
        <router-link tag="button" class="blue-action-button mobile-only" to="/senior-living/our-work">
          <span>View our senior living work  →</span>
        </router-link>
      </div>

      <!-- Home staging section -->
      <div id="home-staging-banner" class="banner-section">
        <div class="banner-image" id="home-staging-image"></div>
        <h2>Home Staging</h2>
        <p>Increase the value of your home with our space planning & design expertise.  </p>
        <router-link tag="button" class="blue-action-button mobile-only" to="/home-staging/our-work">
          <span>View our home staging work  →</span>
        </router-link>
      </div>

    </div>

    <!-- Desktop action buttons -->
    <div id="action-buttons">
      <router-link tag="button" class="blue-action-button desktop-only" to="/senior-living/our-work">
        <span>View our senior living work  →</span>
      </router-link>
      <router-link tag="button" class="blue-action-button desktop-only" to="/home-staging/our-work">
        <span>View our home staging work  →</span>
      </router-link>
    </div>

  </section>
</template>

<script>
import Card from '~/components/Card'

export default {
  name: 'HomePage',

  components: {
    Card
  }
}
</script>

<style scoped lang="scss">

@import '../assets/styles/variables';

#option-banners {
  width: 100%;
  height: 500px;
  display: flex;
  @media screen and (max-width: 1024px) {
    flex-direction: column;
    height: 1000px;
  }
}

.banner-section {
  width: 50%;
  height: 100%;
  overflow: hidden;
  position: relative; /* For the banner image's absolute positioning */
  @media screen and (max-width: 1024px) {
    width: 100%;
    height: 50%;
  }
}
#senior-living-banner {
  
}
.banner-image {
  width: 100%;
  height: 100%;
  background-size: cover;
  filter: brightness(.55);
  transition-duration: .5s;
  position: absolute;
  top: 0;
  left: 0;
}
.banner-section:hover .banner-image {
  transform: scale(1.1);
}
#senior-living-image {
  background-image: url("../assets/senior_living/photo_a.png");
}
#home-staging-image {
  background-image: url("../assets/home_staging/photo_a.png");
}
.banner-section h2 {
  position: relative;
  padding: 275px 50px 0px;
  @media only screen and (max-width: $bp) {
      padding: 155px 50px 0px;

  }
  font-size: 2.5em;
  color: white;
  z-index:10;
  text-shadow: 0px 0px 10px rgba(0,0,0,.7);
}
.banner-section p {
  position: relative;
  color: white;
  font-size: 1.2em;
  z-index:10;
  padding: 10px 50px 0px 50px;
  font-family: CrimsonText;
  text-shadow: 0px 0px 10px rgba(0,0,0,.7);
}
// Action buttons
#action-buttons {
  width: 100%;
  height: 200px;
  display: flex;
  align-items: flex-start;
  justify-content: space-around;
}
.blue-action-button {
  margin-top: 70px;
  font-size: 20px;
  z-index: 100;
  &.mobile-only {
    position: relative;
    margin-left:50px;
  }
}
</style>
