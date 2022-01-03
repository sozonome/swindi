<script lang="ts">
	import DefaultMetaTags from './DefaultMetaTags.svelte';
	import Footer from './Footer.svelte';
	import Header from './Header.svelte';
</script>

<DefaultMetaTags />

<div class="font-sans">
	<Header />
	<main class="layout" py="8">
		<slot />
	</main>
	<Footer />
</div>
