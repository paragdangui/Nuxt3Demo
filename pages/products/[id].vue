<template>
	<div>Product details for {{ id }}</div>
	<p>
		Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ea nostrum
		quisquam, odit mollitia nihil iste vero. Minima atque debitis in?
	</p>
</template>

<script setup>
	const { id } = useRoute().params;

	definePageMeta({
		layout: 'products'
	});
</script>

<style lang="scss" scoped></style>
