<template>
<div class="header-container">
  <header class="the-header">
    <div class="spacer"></div>
    <div class="logo">
      <nuxt-link to="/">
        <img class="img" src="~/assets/images/fitIconlg.png"/>
      </nuxt-link>
    </div>
    <div class="navigation-items">
      <ul class="nav-list">
        <li class="nav-item"><nuxt-link to="/user">Features</nuxt-link></li>
        <li class="nav-item"><nuxt-link to="/user">Partners</nuxt-link></li>
        <li class="nav-item"><nuxt-link to="/user">Pricing</nuxt-link></li>
        <li class="nav-item"><nuxt-link to="/user"><input type="button" class="button" value="Try it free"></nuxt-link></li>
        <li class="nav-item"><nuxt-link to="/user">Login</nuxt-link></li>
        <li class="nav-item"><nuxt-link to="/user">Support</nuxt-link></li>
      </ul>
    </div>
    <div class="spacer"></div>
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
.button {
    background-color: #1B58A5; /* Green */
    border: 1px solid #1B58A5;
    border-radius: 5px;
    color: white;
    padding: 5px 10px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin-right: 100px;
}

.button:hover {
    background-color: #336AAF;
}

.img {
  width: 225px;
  height: 40px;
  padding-right: 20px;
}
.header-container {
  height: 70px;
  font-size: 18px;
  font-family: "adelle-sans",Arial Narrow,Geneva,Lucida Grande,Helvetica,sans-serif;
}

.the-header {
  width: 100%;
  position: fixed;
  height: 70px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  background-color: #1e282d;
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
  color: #bbc5ca;
}

.logo a:hover {
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
  color: #bbc5ca;
}

.nav-item a:hover {
  color: white;
}
</style>
