<template>
  <div>
    <AdminNavBar />
    <nuxt/>
  </div>
</template>

<script>
import AdminNavBar from '@/components/Navigation/AdminNavBar'

export default {
  components: {
    AdminNavBar
  }
}
</script>

<style>
html {
  font-family: "adelle-sans",Arial Narrow,Geneva,Lucida Grande,Helvetica,sans-serif;
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
  color: #262626;
  background-color: white;
}

</style>
