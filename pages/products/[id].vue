<template>
	<div>Product details for {{ id }}</div>
	<p>{{ product.title }}</p>
	<p>{{ product.price }}</p>
	<p>{{ product.id }}</p>
</template>

<script setup>
	const { id } = useRoute().params;
	const uri = 'https://fakestoreapi.com/products/' + id;

	// fetch the products
	const { data: product } = await useFetch(uri,{key: id});

	definePageMeta({
		layout: 'products'
	});
</script>

<style lang="scss" scoped></style>
