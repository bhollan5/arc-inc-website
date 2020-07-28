<template>
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

      <div class="testimonial">
        <h3>Pat F.</h3>
        <p>"To put together room layout, architectural design, color selection and unique accessories, ARC Inc is a gem.  Teresa and Laura were a delight to work as well as true professionals.  Their communication, collaboration and expertise made my entire project go without a hitch.  I would highly recommend them.  My home looks beautiful!!"</p>
      </div>

      <div class="testimonial">
        <h3>Bernard R.</h3>
        <p>"I have really enjoyed working with Teresa and Laura with our new senior living new facility.  We constantly get wonderful compliments from our resident as well as anyone who visits. They always have an upbeat attitude and are not afraid to tackle the difficult issues of design and appealing to the masses.  I wouldn’t hesitate to use ARC Inc again in the future."</p>
      </div>

      <div class="testimonial">
        <h3>John J.</h3>
        <p>"ARC Inc has exceeded all of my expectations with their knowledge of senior living design.  They know all the requirements needed and work efficiently with the contractors.  They produced a beautiful design, on-time, within our budget and with the least disturbance to our residents. We would highly recommend ARC Inc for any of your design needs."</p>
      </div>

      <div class="testimonial">
        <h3>John G.</h3>
        <p>"My wife and I were thinking of selling our home since we are now empty nesters.  We researched the best way to get the greatest return on investment and decided to look into home stagers.  We decided on ARC Inc and couldn’t have been happier with our decision.  Our home ended up looking so beautiful, we fell in love with it all over and again and decided not to sell!  Our kids are happy we decided to stay here as well.  Thank you Teresa and Laura!"</p>
      </div>

    </Flickity>
  </div>
</div>
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
  
}

</script>

<style lang="scss" scoped>
@import '../assets/styles/variables';

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
</style>