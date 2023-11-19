<script>
	import Heading from "$lib/components/heading.svelte";

	export let data;

	console.log(data);

	$: heading = {
		titel: data.websitesData.website.titel,
		homepage: data.urlData.url.url,
		url: data.urlData.url.slug,
	};
</script>

<Heading {heading} />
