<template>
  <section class="container">
    <div>
      <h1 class="title">Fitness Project</h1>
      <h2 class="subtitle">
        another fitness tracker like an ERP system
      </h2>
    </div>
  </section>
</template>

<script>

export default {
  components: {
    
  }
}
</script>

<style>
.container {
  min-height: 10vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  word-spacing: 5px;
  padding-bottom: 15px;
}

</style>
