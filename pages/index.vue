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
  layout: 'admin',
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
  font-family: "adelle-sans",Arial Narrow,Geneva,Lucida Grande,Helvetica,sans-serif;
  display: block;
  font-weight: 300;
  font-size: 60px;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  word-spacing: 5px;
  padding-bottom: 15px;
}

</style>
