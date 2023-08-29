<script>

	const sites = [
		{
			title: "NRK TV",
			url: "https://tv.nrk.no",
			image: 'nrk-tv.webp'
		},
		{
			title: "TV2 Play",
			url: "https://play.tv2.no",
			image: 'tv2-play.webp'
		},
		{
			title: "T-WE",
			url: "https://twe.no",
			image: "t-we.webp"
		},
		{
			title: "HBO MAX",
			url: "https://play.hbomax.com",
			image: "hbo-max.webp"
		},
		{
			title: "Plex",
			url: "https://app.plex.tv",
			image: "plex.webp"
		},

	]

</script>

<ul>
	{#each sites as site}
		<li><a href="https://www.youtube.com/redirect?q={site.url}"><img width=256 src="{site.image}" alt="{site.title}" /></a></li>
	{/each}
</ul>

<style>
	h1 {
		text-align: center;
	}

	img {
		border-radius: 20px;
	}

	ul {
		font-size: 5rem;
		list-style-type: none;
		display: grid;
		grid-template-columns: 1fr 1fr 1fr;
	}
</style>
