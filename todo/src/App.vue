<template>
	
	<div id="app">

		<h1>{{AppMessage}}</h1>

		<nestedone :message="AppMessage" @BubbleOne="AppMessage = $event"></nestedone>

	</div>

</template>

<script>

	import  nestedone from './components/NestedOne';

	export default {
		name: 'app',
		data() {
			return {
				AppMessage: "App Message Here!"
			}
		},
		components: {
			nestedone
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
</style>
