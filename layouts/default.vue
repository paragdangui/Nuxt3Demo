<template>
	<div>
		<header>
			<NuxtLink to="/">Nuxt Website</NuxtLink>
			<nav>
				<ul>
					<li>
						<NuxtLink to="/"> Home </NuxtLink>
						<NuxtLink to="/about"> About </NuxtLink>
						<NuxtLink to="/products"> Products </NuxtLink>
					</li>
				</ul>
			</nav>
		</header>
	</div>

	<div>
		<slot />
	</div>
</template>

<script setup></script>

<style scoped>
	.router-link-exact-active {
		color: #12b488;
	}
</style>
