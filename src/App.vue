<template>
  <div id="app">
    <img src="./assets/logo.png">
		<input class="input" type="search" placeholder="busqueda" v-model="message"></input>
		<Input v-bind:msg="message"/>
		<pre>{{ message }}</pre>
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
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
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
