<template>
  <div id="app">
    <img src="./assets/logo.png">
		<input class="input" type="search" placeholder="busqueda" v-model="message"></input>
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

<style src="./css/style.css"></style>
<!-- <style src="./css/fonts.css"></style> AL PONERLO DA ERROR-->
