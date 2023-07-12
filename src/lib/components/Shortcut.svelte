<script lang="ts">
	import { Avatar } from '@skeletonlabs/skeleton';
	export let name = "Page Name";
	export let href = "/"; // TODO
</script>

<div class="transition-transform  p-2 rounded-xl cursor-pointer hover:bg-surface-500">
	<section class="p-4">
		<Avatar border="rounded-xl w-24" />
	</section>
	<footer class="text-center">{name}</footer>
</div>
