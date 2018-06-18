<template>
	
	<div id="app">

		<nav>
			<router-link to="/">Todo</router-link>
			<router-link :to="{
				path: '/list/0/item/20',
				query: {
					isList: true,
					isItem: false
				}
			}">Item</router-link>

			<button @click=" $router.replace({
					path: '/list/0/item/20',
					query: {
						isList: true,
						isItem: false
					}
				})">
				Route Change
			</button>
		</nav>
		
		<router-view></router-view>

	</div>

</template>

<script>

	export default {
		name: 'app',
		
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
