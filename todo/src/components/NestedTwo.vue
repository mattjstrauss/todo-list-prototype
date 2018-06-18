<template>

	<section>
		
		<h1>{{message}}</h1>
		<button @click=" changeMessage('Bubble two event fired') ">Change Message</button>
	</section>

</template>

<script>
	
	export default {
		name: 'NestedOne',
		props: {
			"message" : {
				type: String,
				required: false,
				default: "Default string"
			}
		},
		methods: {
			changeMessage(message) {
				this.$emit( 'BubbleTwo', message )
			}
		},
	}

</script>