<script>
import Card from '$lib/components/card.svelte';
let cards = [{
        title: 'Cluster map',
        desc: "A map of all students currently in Codam",
        version: "0.2",
        icon: "🗺️",
        href: "1"
    },
    {
        title: 'Students',
        desc: "A list of all students at Codam",
        version: "0.2",
        icon: "🎓",
		href: '2'
    },
    {
        title: 'Coalitions',
        desc: "Statistics on all coalitions at Codam",
        version: "0.2",
        icon: "🪄",
		href: '2'
    },
    {
        title: 'Staff',
        desc: "A list of all staff at Codam",
        version: "0.2",
        icon: "👨‍🏫",
		href: '2'
    }
]
</script>

<svelte:head>
    <title>Home</title>
    <meta name="description" content="Better version of the Codam hero site." />
</svelte:head>

    <!-- <div class="mx-auto">

<h1 class="text-6xl text-center font-black">Hero</h1>
    </div> -->

    <menu class="grid m-5 grid-cols-2 gap-5 my-auto">
		{#each cards as data}
			<Card {...data} />
		{/each}
    </menu>
