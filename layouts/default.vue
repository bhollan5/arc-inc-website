<template>
  <div>
    <b-navbar>
        <template slot="brand">
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                <img
                    src="~assets/arc-logo.png"
                    alt="Arc Inc. logo"
                    height="100"
                >
            </b-navbar-item>
        </template>

        <template slot="end">
          <b-navbar-dropdown label="SENIOR LIVING" hoverable>
                <b-navbar-item href="#">
                    Our Work
                </b-navbar-item>
                <b-navbar-item href="#">
                    Services
                </b-navbar-item>
            </b-navbar-dropdown>
            <b-navbar-dropdown label="HOME STAGING" hoverable>
                <b-navbar-item href="#">
                    Our Work
                </b-navbar-item>
                <b-navbar-item href="#">
                    Services
                </b-navbar-item>
            </b-navbar-dropdown>
            <b-navbar-item href="#">
                US
            </b-navbar-item>
            <b-navbar-item href="#">
                CONTACT
            </b-navbar-item>
        </template>
    </b-navbar>

    <nuxt /> <!-- This is where the route's .vue file is loaded -->

    <div id="footer">
      <div id="footer-content-container">
        <img
            src="~assets/arc-logo.png"
            alt="Arc Inc. logo"
            height="100"
        >
        <div id="site-map" class="footer-section">
          <div class="footer-title">
            SITEMAP
          </div>
          <hr>
          <router-link to="/" class="footer-link" tag="div">
            Home
          </router-link>
          <router-link to="/" class="footer-link" tag="div">
            Senior Living Portfolio
          </router-link>
          <router-link to="/" class="footer-link" tag="div">
            Senior Living Services
          </router-link>
          <router-link to="/" class="footer-link" tag="div">
            Home Staging Portfolio
          </router-link>
          <router-link to="/" class="footer-link" tag="div">
            Home Staging Services
          </router-link>
          <router-link to="/" class="footer-link" tag="div">
            Us
          </router-link>
          <router-link to="/" class="footer-link" tag="div">
            Contact
          </router-link>
        </div>

        <div id="site-map" class="footer-section">
          <div class="footer-title">
            CONTACT
          </div>
          <hr>
          <div>1383 Sharon Coply Rd. P.O. Box 427</div>
          <br>
          <div>tel:     330.239.4474 ext 129</div>
          <div>fax:    330.239.4479</div>
          <br>
          <div>tgresock@hollandmgmt.com</div>
        </div>
      </div>
      <div id="footer-bottom">
        <!-- Add social media icons here -->
         ©  copyright 2019 ARC inc. website design by startup stirfry.
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          title: 'Home',
          icon: 'home',
          to: { name: 'index' }
        },
        {
          title: 'Inspire',
          icon: 'lightbulb',
          to: { name: 'inspire' }
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss" >
@import '../assets/styles/variables';

#footer {
  width: 100%;
  background: $navy;
  color: white;
  img {
    filter: invert(1) brightness(100);
  }
}
#footer-content-container {
  display: flex;
  justify-content: space-around;
  align-items: flex-start;
  padding-top: 100px;

}
.footer-section {
  width: 22%;
  .footer-title {
    font-weight: bold;
  }
}
.footer-link {
  cursor: pointer;
  transition-duration: .5s;
}
.footer-link:hover {
  margin-left: 10px;
}

#footer-bottom {
  text-align: center;
  margin-top: 100px;
}
</style>