<script lang="ts">
	export let title: string;
	export let desc: string;
	export let version: string;
	export let href: string;
	export let icon: string;
</script>

<a
	class="relative block rounded-xl border border-gray-100 p-8 shadow-md hover:shadow-lg hover:scale-[101%] transition-all duration-[400ms]"
	{href}
>
	<span
		class="absolute right-4 top-4 rounded-full bg-green-100 px-3 py-1.5 text-xs font-medium text-green-600"
	>
		v{version}
	</span>

	<div class="mt-4 text-gray-500 sm:pr-8">
		<h1 class="text-5xl">{icon}</h1>

		<h3 class="mt-4 text-xl font-bold text-gray-900">{title}</h3>

		<p class="mt-2 hidden text-sm sm:block">{desc}</p>
	</div>
</a>
