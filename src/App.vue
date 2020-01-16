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
body {
  margin: 0;
  width: 100%;
  height: 100vh;
  font-family: "Barlow", sans-serif;
}

.wrapper {
  width: 100%;
  height: 100%;
  display: flex;
  flex-flow: column;
  justify-content: flex-start;
  overflow: scroll;
}

.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  height: 150px;

  /* background-color: khaki; */
}
.header .menu {
  background-color: hsl(207, 33%, 95%);
}

.logo {
  width: 100%;
  height: 150px;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}
.logo img {
  padding-left: 27%;
}

.menu {
  width: 100%;
  height: 150px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.menu i {
  display: none;
}
ul {
  display: flex;
  align-items: center;
  justify-content: center;
}

ul li {
  display: inline;
  list-style-type: none;
  color: hsl(230, 29%, 20%);
  padding-right: 30px;
  font-family: "Barlow", sans-serif;
  font-weight: 600;
}

li.active {
  color: hsl(231, 7%, 65%);
}

.container {
  display: flex;
  flex-flow: row-reverse;
  height: 100%;
  width: 100%;
}

.text {
  display: flex;
  justify-content: flex-start;
  padding-top: 60px;
  align-items: center;
  flex-flow: column;
  margin-top: 10px;
  width: 50%;
  height: 90%;
}

.text .title {
  font-size: 40px;
  font-weight: 800;
  padding-top: 15px;
  line-height: 10mm;
}

.upper-title {
  width: 300px;
  font-size: 15px;
  /* padding: 15px; */
  color: hsl(231, 7%, 65%);
  font-family: "Barlow", sans-serif;
  padding-bottom: 5px;
}

span {
  background-color: hsl(230, 29%, 20%);
  color: white;
  border-radius: 15px;
  margin-right: 10px;
  font-family: "Barlow", sans-serif;
  font-size: 14px;
  padding: 3px;
  padding-right: 9px;
  padding-left: 9px;
}

.subtitle {
  width: 300px;
  font-size: 12px;
  padding-top: 15px;
  color: hsl(231, 7%, 65%);
}

.illus-img {
  width: 50%;
  height: 40%;
  background-color: hsl(207, 33%, 95%);
  border-bottom-left-radius: 60px;
  text-align: right;
}

.illus-img img {
  width: 100%;
  height: 180%;
  margin-top: 70px;
}

.btn {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 30px;
  width: 100%;
}

.btn-white {
  color: hsl(231, 7%, 65%);
  font-family: "Barlow", sans-serif;
  width: 150px;
  height: 50px;
  border-radius: 5px;
  /* margin: 10px; */
  display: flex;
  align-items: center;
  font-size: 12px;
  justify-content: center;
}

.btn-orange {
  background-color: hsl(0, 100%, 68%);
  font-family: "Barlow", sans-serif;
  width: 150px;
  height: 50px;
  border-radius: 5px;
  font-size: 12px;
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
}
.overlay {
  display: none;
}

@media screen and (max-width: 790px) {
  .wrapper {
    width: 100% !important;
    height: 100%;
  }
  ul {
    display: none;
  }

  .menu {
    justify-content: flex-end;
  }

  .menu i {
    display: inline;
    font-size: 35px;
    padding-right: 27%;
  }

  .menu ul {
    display: none;
  }

  .overlay {
    height: 100%;
    width: 0;
    position: fixed;
    z-index: 1;
    top: 0;
    right: 0;
    background-color: rgb(0, 0, 0);
    background-color: rgba(0, 0, 0, 0.9);
    overflow-x: hidden;
    transition: 0.5s;
  }

  .overlay-content {
    position: relative;
    top: 25%;
    width: 100%;
    text-align: center;
    margin-top: 30px;
  }

  .overlay a {
    padding: 8px;
    text-decoration: none;
    font-size: 36px;
    color: #818181;
    display: block;
    transition: 0.3s;
  }

  .overlay a:hover,
  .overlay a:focus {
    color: #f1f1f1;
  }

  .overlay .closebtn {
    position: absolute;
    top: 20px;
    right: 45px;
    font-size: 60px;
  }
  .container {
    display: flex;
    flex-flow: column;
    align-items: center;
    justify-content: flex-start;
  }

  .container .text {
    display: flex;
    align-items: center;
    text-align: left;
    justify-content: center;
    flex-flow: column;
    width: 100%;
    height: 90%;
    padding-top: 30px;
  }

  .subtitle {
    width: 350px;
    font-size: 10px;
    color: hsl(231, 7%, 65%);
  }

  .upper-title {
    width: 350px;
  }

  .title {
    width: 350px;
    font-size: 10px;
  }
  .btn {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: 30px;
    width: 100%;
  }

  .btn-white {
    color: hsl(231, 7%, 65%);
    font-family: "Barlow", sans-serif;
    width: 150px;
    height: 50px;
    border-radius: 5px;
    margin: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .illus-img {
    width: 100%;
    height: 90%;
    background-image: linear-gradient(
      to right,
      white 50%,
      hsl(207, 33%, 95%) 50%
    );
    border-radius: 10px;
  }

  .illus-img img {
    width: 100%;
    height: 80%;
  }

  .btn-orange {
    background-color: hsl(0, 100%, 68%);
    font-family: "Barlow", sans-serif;
    width: 150px;
    height: 50px;
    border-radius: 5px;
    margin-right: 10px;
    margin-top: 10px;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .title {
    color: hsl(230, 29%, 20%);
    font-size: 28px;
    font-weight: 800;
    font-family: "Barlow", sans-serif;
  }

  .subtitle {
    color: hsl(231, 7%, 65%);
    font-size: 18px;
  }

  .overlay {
    height: 100%;
    width: 0;
    position: fixed;
    z-index: 1;
    top: 0;
    right: 0;
    background-color: rgb(0, 0, 0);
    background-color: rgba(0, 0, 0, 0.9);
    overflow-x: hidden;
    transition: 0.5s;
  }

  .overlay-content {
    position: relative;
    top: 25%;
    width: 100%;
    text-align: center;
    margin-top: 30px;
  }

  .overlay a {
    padding: 8px;
    text-decoration: none;
    font-size: 36px;
    color: #818181;
    display: block;
    transition: 0.3s;
  }
}

@media screen and (max-width: 300px) {
  .btn {
    flex-flow: column;
    align-items: center;
    justify-content: center;
    width: 100%;
  }
}

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
