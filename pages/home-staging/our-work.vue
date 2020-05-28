
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
        <img src="../../assets/home_staging/new/home_staging_3.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/home_staging/new/home_staging_4.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/home_staging/new/home_staging_5.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/home_staging/new/home_staging_6.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/home_staging/new/home_staging_7.jpg">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/home_staging/new/home_staging_8.jpg">
      </div> 

    </div>

    <router-link to="/home-staging/services" tag="button" class="blue-action-button">
        See our home staging services →
    </router-link>

    <div id="testimonials">
      <h2>Testimonials</h2>
      <hr>
      <div class="flickity-container">
        <Flickity :options="flickityOptions" ref="flick">
          <div class="testimonial">
            <h3>Tony Maroni, LNHA</h3>
            <p>"ARC designed our dining room. We get compliments on it daily. Our residents and staff are extremely pleased with functionality of the space. On a personal level, working with the designer Teresa is a pleasure to deal with and she is a great communicator, very talented with great creative ideas.  They were able to work within a set budget to help control costs. We look forward to working with ARC again soon!"</p>
          </div>
          <div class="testimonial">
            <h3>Cathie Miles, Smith Center</h3>
            <p>"ARC INC. designs rocked the transformation of the entrance and community room with elegance and color. Working with designer Teresa was an outstanding experience with great communication. Thank you, ARC INC. you have been a source of inspiration to the Smith Center."</p>
          </div>
          <div class="testimonial">
            <h3>Melissa Frank-Elwell, Martin House</h3>
            <p>"ARC, Inc. has done an exceptional job with our renovations here. The quality of the designs, the colors and the professionalism of the team at ARC, Inc. has been wonderful. Everyday, our residents, families, and business associates comment on how beautiful our facility looks from the renovations that were completed by ARC, Inc and their team. Thank you for making our residents smile every day!"</p>
          </div>
        </Flickity>
      </div>
    </div>
  </section>
</template>

<script>

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
