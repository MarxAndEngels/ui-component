<template lang="">
    <div>
        <nav class="navbar navbar-dark bg-dark navbar-expand-lg">
  <div class="container">
     <nuxt-link to="/">  <a class="navbar-brand" href="">Ui component</a> </nuxt-link>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarScroll" aria-controls="navbarScroll" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarScroll">
      <ul class="navbar-nav me-auto my-2 my-lg-0 navbar-nav-scroll" style="--bs-scroll-height: 100px;">
      </ul>

      <!-- <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form> -->
    </div>
  </div>
</nav>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    a{
        color: snow;
        text-decoration: none;
    }
    a:hover{
        color: rgb(163, 161, 161);
        text-decoration: none;
    }

</style>