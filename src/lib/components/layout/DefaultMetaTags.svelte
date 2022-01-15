<script lang="ts">
	import { MetaTags } from 'svelte-meta-tags';
	import { page } from '$app/stores';

	const {
		stuff: { seo }
	} = $page;
</script>

<MetaTags
	title={seo?.title ?? 'swindi'}
	description={seo?.description ?? 'Svelte Kit starter template with WindiCSS setup'}
	canonical="https://swindi.sznm.dev"
	openGraph={seo?.openGraph ?? {
		url: 'https://swindi.sznm.dev',
		title: 'Svelte Kit + WindiCSS',
		description: 'Svelte Kit starter template with WindiCSS setup',
		site_name: 'swindi'
	}}
	twitter={seo?.twitter ?? {
		handle: '@sozonome',
		site: 'https://sznm.dev',
		cardType: 'summary_large_image'
	}}
/>
