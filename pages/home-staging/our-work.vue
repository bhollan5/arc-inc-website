
<template>
  <section>
    <div class="image-banner">
      <img src="../../assets/home_staging/photo_a.png">
      <h1>Our home staging increases your home's value.</h1>
    </div>
    <div class="blue-subtitle">
      Our interior design specialists know how to sell a house. 
    </div>

    <div class="image-gallery">
      <Flickity :options="flickityOptions" ref="flick">

        <div class="gallery-image-container">
          <img src="../../assets/home_staging/gallery/Akron.jpg">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/gallery/akron2.jpg">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/gallery/akron4.jpg">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/gallery/akron7.jpg">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/gallery/dover-035.jpg">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/gallery/IMG_1120.JPG">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/gallery/P1020764.JPG">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/gallery/photo_c.jpg">
        </div>

        <!-- New -->

        <div class="gallery-image-container">
          <img src="../../assets/home_staging/new/home_staging_1.jpg">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/new/home_staging_2.jpg">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/new/home_staging_3.JPG">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/new/home_staging_4.JPG">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/new/home_staging_5.jpg">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/new/home_staging_6.JPG">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/new/home_staging_7.jpg">
        </div>
        <div class="gallery-image-container">
          <img src="../../assets/home_staging/new/home_staging_8.jpg">
        </div> 

      </Flickity>

    </div>

    <router-link to="/home-staging/services" tag="button" class="blue-action-button">
        See our home staging services →
    </router-link>

    <!-- Using our testimonials component -->
    <testimonials></testimonials>

  </section>
</template>

<script>
import testimonials from '~/components/testimonials.vue';

export default {
  name: 'seniorWork',
  data() {
    return {
      flickityOptions: {
        initialIndex: 3,
        prevNextButtons: false,
        pageDots: true,
        wrapAround: true
      }
    }
  },

  mounted() {
      setTimeout(() => this.$refs.flick.reloadCells(), 1500);
  },
  components: {
    testimonials
  }
}
</script>

<style scoped lang="scss">
@import '../../assets/styles/variables';

button {
    margin-left: 50%;
    transform: translatex(-50%);
    margin-top: 50px;
    margin-bottom: 50px;
    min-width: 100px;
    display: block;
  }


flickity { display: block; }
.flickity { display: block; }

.image-banner {
  height: 400px;
  width: 100%;
  h1 {
    margin-top: 80px;
  }

  @media only screen and (max-width: $bp) {
    height: 200px;
    h1 {
      font-size: 1.7em;
      width: 100%;
      margin-top: 40px;
    }
  }
  img {
    filter: brightness(65%);
    margin-top: -150px;
    @media only screen and (max-width: $bp) {
      margin-top: 0px;
      object-fit: cover;
    }
  }
}
.blue-subtitle {
  width: 100%;
  padding: 20px;
  background: $navy;
  text-align: center;
  color: white;
}

.image-gallery {
  width: 100%;
  height: 550px;
  padding: 50px 5%;
  text-align: center;
  .gallery-image-container {
    height: 400px;
    width: 100%;
    margin-bottom: 50px;
    margin-top: 50px;
    img {
      height: 100%;
      transition-duration: .5s;
    }
    img:hover {
      height: 110%;
      margin-top: -5%;
    }
  }
}



.rotate {
  transform: rotate(90deg);
}
</style>
