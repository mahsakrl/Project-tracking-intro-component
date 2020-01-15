<template>
  <div class="wrapper">
    <div class="header">
      <div class="logo">
        <img src="./assets/images/logo.svg" />
      </div>
      <div id="myNav" class="overlay">
        <a href="javascript:void(0)" class="closebtn" @click="closeNav()">&times;</a>
        <div class="overlay-content">
          <a href="#">Login</a>
          <a href="#">Pricing</a>
          <a href="#">Feature</a>
          <a href="#">Product</a>
        </div>
      </div>
      <div class="menu">
        <i class="material-icons" @click="openNav()">menu</i>
        <ul>
          <li>Product</li>
          <li>Feature</li>
          <li>Pricing</li>
          <li class="active">Login</li>
        </ul>
      </div>
    </div>
    <div class="container">
      <div class="illus-img">
        <img src="./assets/images/illustration-devices.svg" />
      </div>
      <div class="text">
        <div class="upper-title">
          <span>New</span>Monograph & nbsp Dashboard
        </div>
        <div class="title">
          Powerful insights
          <br />into your team
        </div>
        <div class="subtitle">
          Project planning and time tracking
          <br />for agile teams
        </div>
        <div class="btn">
          <div class="btn-orange">SCHEDULE A DEMO</div>
          <div class="btn-white">TO SEE A PREVIEW</div>
        </div>
      </div>
    </div>
  </div>
</template>
<style>
@import url('./assets/style/index.css');
</style>
<script>
export default {
  methods: {
    openNav () {
      document.getElementById('myNav').style.width = '100%'
    },

    closeNav () {
      document.getElementById('myNav').style.width = '0%'
    }
  }
}
</script>
