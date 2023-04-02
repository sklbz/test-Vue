<template>
	<section>
		<p v-if="likes>0">
			THIS HAS {{ likes }} 👍
		</p>
		<p v-else>
			nobody likes this
		</p>

		<button v-on:click="likes++">Click Me</button>
	</section>
</template>

<script>
	export default {
		data() {
			return {
				likes: 0,
			}

		}
	}
</script>