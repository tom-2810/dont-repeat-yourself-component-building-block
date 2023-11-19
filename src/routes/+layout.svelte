<script>
	import Header from "$lib/components/header.svelte";
	import "../global.css";

	import { page } from "$app/stores";
	export let data;
	$: params = $page.params;

	let partners = data.partnersData;
	$: websites = data.websitesData.website;
</script>

<Header {params} {partners} {websites} />
<main>
	<slot />
</main>
