<script lang="ts">
import About from '$lib/components/About/index.svelte';

	import Logs from '$lib/components/Logs.svelte';
	import Main from '$lib/components/Main.svelte';
	import { selectedTab } from '$lib/store';

	let currentTab: number;

	selectedTab.subscribe((v) => (currentTab = v));
</script>

<Main />

{#if currentTab == 0}
	<About />
{:else}
	<Logs />
{/if}
