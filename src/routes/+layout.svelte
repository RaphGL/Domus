<script lang="ts">
	// The ordering of these imports is critical to your app working properly
	import '@skeletonlabs/skeleton/themes/theme-crimson.css';
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Most of your app wide CSS should be put in this file
	import '../app.postcss';
	import { AppShell, AppBar, TabGroup, TabAnchor, Tab } from '@skeletonlabs/skeleton';
	import { page } from '$app/stores';

    let addTab = false;
</script>

<!-- App Shell -->
<AppShell>
	<svelte:fragment slot="header">
		<AppBar>
			<svelte:fragment slot="lead">
				<TabGroup justify="justify-center">
					<TabAnchor href="/" selected={$page.url.pathname === '/'}>Home</TabAnchor>
					<TabAnchor href="/custom" selected={$page.url.pathname === '/custom'}>Custom</TabAnchor>
				</TabGroup>
                <button type="button" class="ml-2 btn btn-sm variant-filled-surface">+</button>
			</svelte:fragment>

			<svelte:fragment slot="trail">
				<button type="button" class="btn variant-filled-surface">Settings</button>
			</svelte:fragment>
		</AppBar>
	</svelte:fragment>
	<!-- Page Route Content -->
	<slot />
</AppShell>
