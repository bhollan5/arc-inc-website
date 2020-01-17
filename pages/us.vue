<template>
  <section>
    <div id="us">
      <h1>Great design takes a great team.</h1>
      <hr><br><br>
      
      <div class="bio" v-for="person in staff">
        <img :src="`/bio_images/${person.img}`">
        <div class="bio-text">
          <h3>{{person.name}}</h3>
          <p class="bio-title">{{person.title}}</p>
          <br><br>
          <p v-for="line in person.bio">{{line}}</p>
          <br><br>
          <p style="display: flex;align-items: center;">
            <img src="@/assets/icons/mail.png" width="25" style="margin-right:10px;">
            <a :href="'mailto:' + person.email" style="margin-top: 0px;">
              {{person.email}}
            </a>
          </p>
        </div>
      </div>

    </div>
    
  </section>
</template>

<script>

export default {
  name: 'seniorServices',
  data() {
    return {
      staff: [
        {
          name: "Teresa Holland",
          title: "Project Principal",
          bio: ["Teresa started ARC inc. in 200X. She's proud to have worked in an executive design role  on all the company's major projects. ",
          "Teresa graduated from Kent State University with a BA in Interior Architecture."],
          img: "teresa.jpg",
          email: "tgresock@hollandmgmt.com"
        },
        {
          name: "Laura Wack",
          title: "Lead Interior Designer",
          bio: ["[ Bio here! ]"],
          img: "laura.jpg",
          email: "lwack@hollandmgmt.com"
        },
        {
          name: "Don Funk",
          title: "Architecture consultant",
          bio: ["[ Bio here! ]"],
          img: "don.jpg",
          email: "dfunk@hollandmgmt.com"
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/variables';

#us {
  background: $navy;
  color: white;
  padding: 50px 10%;
  min-height: 100vh;
}
h1 {
  font-size: 3em;
}

.bio {
  display: flex;
  flex-flow: row wrap;
  font-family: CrimsonText;
  margin-bottom: 100px;
  img {
    margin-right: 30px;
    max-height: 300px;
    max-width: 300px;
  }
  h3 {
    font-size: 30px;
    font-weight: bold;
  }
  p:not(.bio-title) {
    font-size: 18px;
  }
  a {
    color: white;
    text-decoration: underline;
  }
}

</style>
