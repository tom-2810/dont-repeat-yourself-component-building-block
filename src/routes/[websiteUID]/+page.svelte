<script>
	import Heading from "$lib/components/heading.svelte";

	export let data;

	$: heading = {
		titel: data.websitesData.website.titel,
		homepage: data.websitesData.website.homepage,
	};
</script>

<Heading {heading} />
