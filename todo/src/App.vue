<template>
	
	<div id="app">

		<h1>{{name}}</h1>

		<nestedone :message="name" @BubbleOne=" $store.dispatch( 'changeName', $event ) "></nestedone>

	</div>

</template>

<script>

	import  nestedone from './components/NestedOne';

	export default {
		name: 'app',
		computed: {
			name(){
				return this.$store.state.firstName + ' ' + this.$store.state.lastName;
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
