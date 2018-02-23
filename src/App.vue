<template>
  <div id="app">
    <img src="./assets/logo.png">
		<h1>Hello Vue Component</h1>
		<input class="input" type="search" placeholder="busqueda" v-model="message"/>
		<Input v-bind:msg="message"/>
		<!-- <pre>{{ message }}</pre> -->
  </div>
</template>

<script>
import Input from './components/Input'

export default {
  name: 'App',
  components: {
		Input
  },
	data() {
		return {
			message: ''
		}
	}
}
</script>

<style>
@import url('./fonts/stylesheet.css'); 

* {
	margin: 0;
	box-sizing: border-box;
	font-family: 'Avenir Next LT Pro', serif;
}

#app {
	font-weight: 900;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.input {
	border: 1px solid black;
}
</style>