<template>
<div class="header-container">
  <header class="the-header">
    <div class="logo">
      <nuxt-link to="http://www.facebook.com"><font-awesome-icon :icon="fb" fixed-width /></nuxt-link> 
      <nuxt-link to="http://www.twitter.com"><font-awesome-icon :icon="tw" fixed-width /></nuxt-link>
      </div>
    <div class="spacer"></div>
    <div class="navigation-items">
      <ul class="nav-list">
        <li class="nav-item"><nuxt-link to="/">Blog</nuxt-link></li>
        <li class="nav-item"><nuxt-link to="/">About</nuxt-link></li>
        <li class="nav-item"><nuxt-link to="/">Admin</nuxt-link></li>
      </ul>
    </div>
  </header>
</div>
</template>

<script>
import FontAwesomeIcon from '@fortawesome/vue-fontawesome'
import { faFacebookF } from '@fortawesome/fontawesome-free-brands'
import { faTwitter } from '@fortawesome/fontawesome-free-brands'

export default {
  name: 'TopNavBar',
  computed: {
      fb () {
          return faFacebookF
      },
      tw () {
          return faTwitter
      }
  },
  components: {
      FontAwesomeIcon
  }
}
</script>


<style scoped>
.header-container {
  height: 40px;
}

.the-header {
  width: 100%;
  position: fixed;
  height: 40px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  background-color: #0B3C5D;
  z-index: 100;
  box-sizing: border-box;
  padding: 0 20px;
}

.logo {
  margin: 0 10px;
  font-size: 1.3rem;
}

.logo a {
  text-decoration: none;
  color: white;
}

.spacer {
  flex: 1;
}

.navigation-items {
  display: none;
}

@media (min-width: 768px) {
  .navigation-items {
    display: block;
  }
}

.nav-list {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
}

.nav-item {
  margin: 0 10px;
}

.nav-item a {
  text-decoration: none;
  color: black;
}

.nav-item a:hover,
.nav-item a:active,
.nav-item a.nuxt-link-active {
  color: white;
}
</style>
