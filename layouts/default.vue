<template>
  <div>
    <TopNavBar />
    <MainNavBar />
    <nuxt/>
  </div>
</template>

<script>
import TopNavBar from '@/components/Navigation/TopNavBar'
import MainNavBar from '@/components/Navigation/MainNavBar'

export default {
  components: {
    TopNavBar,
    MainNavBar
  }
}
</script>

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

body {
  margin: 0;
  color: white;
  background-color: #192231;
}

</style>
