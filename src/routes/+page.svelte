<script>
	import Card from '$lib/components/card.svelte';
	let cards = [
		{
			title: 'Cluster map',
			desc: 'A map of all students currently in Codam',
			version: '0.2',
			icon: '🗺️',
			href: '/'
		},
		{
			title: 'Students',
			desc: 'A list of all students at Codam',
			version: '0.2',
			icon: '🎓',
			href: '/'
		},
		{
			title: 'Coalitions',
			desc: 'Statistics on all coalitions at Codam',
			version: '0.2',
			icon: '🪄',
			href: '/'
		},
		{
			title: 'Staff',
			desc: 'A list of all staff at Codam',
			version: '0.2',
			icon: '👨‍🏫',
			href: '/'
		}
	];
</script>

<svelte:head>
	<title>CodamHero</title>
	<meta name="description" content="my version of the Codam hero site." />
</svelte:head>

<menu class="grid m-5 grid-cols-2 gap-5 my-auto">
	{#each cards as data}
		<Card {...data} />
	{/each}
</menu>
