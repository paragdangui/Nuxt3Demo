<template>
	<div class="grid grid-cols-4 gap-5">
		<div v-for="p in products"></div>
		<ProductCard :product="p" />
	</div>
</template>

<script setup>
	definePageMeta({
		layout: 'products'
	});

	// fetch the products
	const { data: products } = await useFetch(
		'https://fakestoreapi.com/products'
	);
</script>

<style lang="scss" scoped></style>
