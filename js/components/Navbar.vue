<template>

<nav class="navbar navbar-light bg-light">
  <a class="navbar-brand" href="#">
    <img class="rounded-circle" height="40" width="40" :src="image" alt="">
    VueJS
  </a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" aria-controls="navbarNav"  aria-label="Toggle navigation">
  <span class="navbar-toggler-icon"></span>
  </button>
  
</nav>

</template>

<script>
module.exports = {

  data() {
  	return {
  		image: '../static/images/nav.png'
  	}
  },	

  mounted () {
    console.log('this is a navbar')
  }
};
</script>

<style scoped>
span {
  background-color: yellow;
}
</style>