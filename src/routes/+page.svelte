<script>
	import { Avatar } from '@skeletonlabs/skeleton';
	import Shortcut from '$lib/components/Shortcut.svelte';
</script>

<!-- YOU CAN DELETE EVERYTHING IN THIS PAGE -->
<div class="flex flex-col gap-8 justify-center h-full items-center w-screen">
	<h1 class="h1 h-28"><b>Domus</b></h1>

	<input
		class="input autocomplete p-2 w-full w-1/2 text-center"
		type="search"
		name="autocomplete-search"
		placeholder="Search..."
	/>

	<div class="flex gap-4">
		<Shortcut name="YouTube" />
		<Shortcut name="9Anime" />
		<Shortcut name="GitHub" />
		<Shortcut name="StackOverflow" />
	</div>
</div>
