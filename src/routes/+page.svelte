<script>
	import Card from '$lib/components/card.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Better version of the Codam hero site." />
</svelte:head>

<div class="mx-auto">
	<h1 class="text-6xl text-center font-black">Hero</h1>
</div>

<menu class="grid m-5 grid-cols-2 gap-5 my-auto">
	<Card
		title="Cluster map"
		desc="A map of all students currently in Codam"
		version="0.2"
		icon="🗺️"
		href="1"
	/>
	<Card
		title="Students at Codam"
		desc="A list of all the students currently at Codam"
		version="0.1"
		icon="🎓"
		href="2"
	/>
	<Card
		title="Coalitions"
		desc="Statistics on all coalitions at Codam"
		version="0.1"
		icon="🪄"
		href="3"
	/>
	<Card title="Staff" desc="A list of all staff at Codam" version="0.1" icon="🏫" href="4" />
</menu>
