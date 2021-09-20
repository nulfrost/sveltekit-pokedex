<script>
	export let pokeman;
	import { fade } from 'svelte/transition';
</script>

<a
	href={`/pokemon/${pokeman.id}`}
	class="list-none p-6 bg-gray-100 text-gray-800 text-center rounded-md shadow-sm hover:shadow-md flex flex-col items-center"
	transition:fade
>
	<img src={pokeman.image} alt={pokeman.name} class="h-40 w-40" />
	<h2 class="uppercase">{pokeman.id}. {pokeman.name}</h2>
</a>
