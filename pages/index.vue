<template>
  <section>
    <div id="option-banners">
      <div id="senior-living-banner" class="banner-section">
        <div class="banner-image" id="senior-living-image"></div>
        <h2>Senior Living</h2>
        <p>For decades, ARC Inc. has been designing thoughtful, dignified spaces for the senior living community. </p>
      </div>
      <div id="home-staging-banner" class="banner-section">
        <div class="banner-image" id="home-staging-image"></div>
        <h2>Home Staging</h2>
        <p>Increase the value of your home with our space planning & design expertise.  </p>
      </div>
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

<style scoped>
#option-banners {
  width: 100%;
  height: 500px;
  display: flex;
}
.banner-section {
  width: 50%;
  height: 100%;
  overflow: hidden;
  position: relative; /* For the banner image's absolute positioning */
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
  padding: 45% 50px 0px;
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
</style>
