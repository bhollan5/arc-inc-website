<template>
  <section>
    <div class="image-banner">
      <img src="../../assets/senior_living/our_work_banner.png">
      <h1>Creating dignified senior living environments is our specialty.</h1>
    </div>
    <div class="blue-subtitle">
      ARC Inc. has been designing thoughtful, dignified senior spaces for decades. 
    </div>
    <div class="image-gallery">
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_1.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_2.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_3.png">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_4.png">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_5.png">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_6.png">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_7.png">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_8.png">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_9.png">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_10.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_11.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_12.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_13.jpg">
      </div>
      <!--<div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_14.jpg">
      </div>-->
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_15.jpg">
      </div>

      <!-- New additions: -->
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_16.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_17.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_18.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_19.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_20.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_21.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_22.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_23.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_24.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_25.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_26.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_27.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_28.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_29.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_30.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_31.JPG">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/new_additions/senior_living_gallery_32.JPG">
      </div>
      

    </div>

    <router-link to="/senior-living/services" tag="button" class="blue-action-button">
        See our senior living services →
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
  padding: 50px 5%;
  display: flex;
  justify-content: space-around;
  flex-flow: row wrap;
  .gallery-image-container {
    width: 400px;
    height: 400px;
    overflow: hidden;
    margin-bottom: 50px;
    img {
      height: 100%;
      object-fit:cover;
      transition-duration: .5s;
    }
    img:hover {
      height: 110%;
      margin-top: -5%;
    }
  }
}

#testimonials {
  text-align: center;
  background: $tan;
  color: $navy;
  padding:  50px 10%;
  h2 {
    font-size: 40px;
  }
  
}
hr {
    background: $navy;
  }

.testimonial {
  width: 425px;
  max-width: 100%;
  height: 310px;
  background: white;
  padding: 40px 20px;
  margin: 20px;
  @media only screen and (max-width: $bp) {
    height: 400px;
  }
  h3 {
    font-size: 22px;
    font-weight: bold;
    margin-bottom: 30px;
  }
}
.flickity-container {
  width: 100%;
}

.rotate {
  transform: rotate(90deg);
}
</style>
