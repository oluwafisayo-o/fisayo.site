<template>
	<h1 v-if="text" class="title" v-html="text" />
</template>

<script>
export default {
	props: {
		text: {
			type: String,
			required: false,
		},
	},
};
</script>

<style scoped>
.title {
	/* text-align: center; *-moz-animation; */
	font-size: /*3.6rem;*/ calc(21px + (48 - 14) * ((100vw - 300px) / (1600 - 300)));
	font-weight: 500;
	line-height: 1.4;
	letter-spacing: -0.05rem; /* 0.1rem; */
	width: 80vw /*800px*/;
	max-width: 100%;
	margin: 8rem 0; /*5rem auto 7vw 0;*/
	padding: 0; /*2rem 0 0 0;*/
}

@media screen and (min-width: 600px) {
	.title {
		/* margin: 12vw auto 7vw 0vw;
		width: 100%;
		padding: 3.2rem 0 0 0; */

		margin: 8rem 0;
		width: 80%;
		padding: 0;
	}
}
</style>
