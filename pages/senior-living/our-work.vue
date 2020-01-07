<template>
  <section>
    <div class="image-banner">
      <img src="../../assets/senior_living/our_work_banner.png">
      <h1>Creating dignfied senior living environments is our specialty.</h1>
    </div>
    <div class="blue-subtitle">
      ARC Inc. has been designing thoughtful, dignified senior spaces for decades. 
    </div>
    <div class="image-gallery">
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_2.png">
      </div>
      <div class="gallery-image-container">
        <img src="../../assets/senior_living/gallery/senior_living_gallery_1.png">
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
    </div>
    <div id="testimonials">
      <h2>Testimonials</h2>
      <hr>
      <div class="flickity-container">
        <Flickity :options="flickityOptions">
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
  components: {
  }
}
</script>

<style scoped lang="scss">
@import '../../assets/styles/variables';

.image-banner {
  height: 400px;
  img {
    filter: brightness(65%);
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
  height: 310px;
  background: white;
  padding: 40px 20px;
  margin: 20px;
  h3 {
    font-size: 22px;
    font-weight: bold;
    margin-bottom: 30px;
  }
}
.flickity-container {
  width: 100%;
}
</style>
