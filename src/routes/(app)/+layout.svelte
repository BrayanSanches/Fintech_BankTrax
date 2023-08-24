<script lang='ts'>
	// The ordering of these imports is critical to your app working properly
	import '@skeletonlabs/skeleton/themes/theme-skeleton.css';
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Most of your app wide CSS should be put in this file

	import { AppShell } from '@skeletonlabs/skeleton';
	import Header from '../../lib/components/header.svelte';
</script>

<AppShell class="w-screen h-screen bg-gray-100 dark:bg-surface-700	">
	<svelte:fragment slot="header"> <Header></Header> </svelte:fragment>
	<!-- (sidebarLeft) -->
	<!-- (sidebarRight) -->
	<!-- (pageHeader) -->
	<!-- Router Slot -->
	<slot />
	<!-- ---- / ---- -->
	<!-- (pageFooter) -->

</AppShell>
