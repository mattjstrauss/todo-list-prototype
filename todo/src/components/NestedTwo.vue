<template>

	<section>
		
		<h1>{{name}}</h1>
		<button @click=" $store.dispatch('changeName', 'Bubble twoclisdfsdfcked') ">Change Message</button>
	</section>

</template>

<script>
	
	export default {
		name: 'NestedOne',
		computed: {
			name(){
				return this.$store.state.firstName + ' ' + this.$store.state.lastName;
			}
		},
	}

</script>