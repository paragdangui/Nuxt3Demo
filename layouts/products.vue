<template>
	<div>
		<header>
			<NuxtLink to="/products">Nuxt Merch</NuxtLink>
			<nav></nav>
		</header>
		<div>
			<slot />
		</div>
		<footer>
			<ul>
				<li>
					<NuxtLink to="/"> Home </NuxtLink>
					<NuxtLink to="/about"> About </NuxtLink>
					<NuxtLink to="/products"> Products </NuxtLink>
				</li>
			</ul>
		</footer>
	</div>
</template>

<script setup></script>

<style scoped>
	.router-link-exact-active {
		color: #12b488;
	}
</style>
