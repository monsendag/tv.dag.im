<script>

	const sites = [
		{
			title: "NRK TV",
			url: "https://tv.nrk.no"
		},
		{
			title: "TV2 Play",
			url: "https://play.tv2.no"
		},
		{
			title: "T-WE",
			url: "https://twe.no"
		},
		{
			title: "HBO MAX",
			url: "https://play.hbomax.com"
		},
		{
			title: "Plex",
			url: "https://app.plex.tv"
		},

	]

</script>
<h1>Streaming sites</h1>

<ul>
	{#each sites as site}
		<li><a href="https://www.youtube.com/redirect?q={site.url}">{site.title}</a></li>
	{/each}
</ul>

<style>
	h1 {
		text-align: center;
	}

	ul {
		font-size: 5rem;
		list-style-type: none;
		display: grid;
		grid-template-columns: 1fr 1fr 1fr;
	}
</style>
