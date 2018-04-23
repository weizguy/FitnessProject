<template>
<div class="header-container">
  <header class="the-header">
    <div class="logo">
      <nuxt-link to="/">FITNESS KEEPER</nuxt-link>
    </div>
    <div class="spacer"></div>
    <div class="navigation-items">
      <ul class="nav-list">
        <li class="nav-item"><nuxt-link to="/user">User</nuxt-link></li>
        <li class="nav-item"><nuxt-link to="/diet">Diet</nuxt-link></li>
        <li class="nav-item"><nuxt-link to="/exercise">Exercise</nuxt-link></li>
      </ul>
    </div>
  </header>
</div>
</template>

<script>

export default {
  name: "MainNavBar",
  components: {

  }
};
</script>


<style scoped>
.header-container {
  height: 100px;
}

.the-header {
  width: 100%;
  position: fixed;
  height: 100px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  background-color: #D9B310;
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
  color: black;
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
