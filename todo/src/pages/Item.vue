<template>

	<section>

		<button @click=" $router.go(-1) ">Go Back</button>
	
		<pre>
			
			Params: listId = {{ listID }}, itemId = {{ itemID}}
			Query: isList = {{ $route.params.isList }}, isItem = {{ $route.params.isItem }}

		</pre>

	</section>

</template>

<script>
	
	export default {
		name: 'Item',
		props: [ "listID", "itemID" ]
	}

</script>

<style>
	
</style>