<template>
  <div id="app">
    <div class="nav">
      <img src="./assets/logo.png" alt>
      <ul>
        <li>I am a consumer</li>
        <li>Explore photos</li>
        <li>Find a photographer</li>
        <li>Join the community</li>
        <li class="active">Login or register</li>
      </ul>
    </div>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: "app",
  components: {}
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Lora|Montserrat&display=swap");
$base-color: #fbb503;
* {
  box-sizing: border-box;
}
body {
  padding: 0;
  margin: 0;
  width: 100% !important;
  overflow-x: hidden;
  font-family: "Montserrat", sans-serif;
  font-weight: 400;
}
.heading {
  font-family: "Lora", serif;
}
.nav {
  /* width: 100% !important; */
  height: 70px;
  line-height: 70px;
  background-color: #4d4d4d;
  padding: 0 30px;
}
.nav img {
  height: 50px;
  margin-top: 10px;
  float: left;
}
ul {
  float: right;
  height: 70px;
  line-height: 70px;
  margin: 0;
  padding: 0;
}
li {
  list-style: none;
  display: inline;
  padding: 12px;
  font-size: 14px;
  color: #fff;
}
li.active {
  color: $base-color;
}

.mt20 {
  margin-top: 20px;
}
.yellow-btn {
  background-color: $base-color;
  color: #4d4d4d;
  border: 0;
  border-radius: 100px;
  padding: 12px 40px;
  font-size: 18px;
}
</style>
