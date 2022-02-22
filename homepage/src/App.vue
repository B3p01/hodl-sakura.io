<template>
  <NavBar />
  <Homepage />
</template>

<script>
import NavBar from './components/NavBar.vue'
import Homepage from './components/HomePage.vue'
//import aos from './assets/js/aos'


export default {
  name: 'App',
  components: {
    Homepage,
    NavBar
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
:root {
	--primary: transparent;
	--primary-light: #212d37;
	--secondary: #db0303;
	--tertiary: #990606 ;
	--gradient: linear-gradient(to right, #f7ff6e, #f95519);
}
html, body {width: auto!important; overflow-x: hidden!important; } 
h1,
h2,
h3,
h4,
h5,
h6 {
	font-family: "samurai", sans-serif;
}
@import url('https://fonts.googleapis.com/css?family=Open+Sans');
.opensans {
  font-family: "Open Sans", sans-serif;
}
@font-face {
	font-family: 'samurai';
	src: url(@/assets/webfonts/BLACKFIGHTER.woff);
}
h1 {
	font-size: 40px;
	font-weight: 400;
}
button {
	font-family: sans-serif;
}
p {
	margin: 0;
	padding: 0;
	font-family: 'Open Sans';
	font-size: 20px;
}
ul,
h4 {
	margin: 0;
	padding: 0;
}
a {
	color: white;
	text-decoration: none;
}
</style>
