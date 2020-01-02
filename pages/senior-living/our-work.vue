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
  </section>
</template>

<script>

export default {
  name: 'seniorWork',

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
</style>
