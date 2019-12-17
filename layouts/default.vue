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
