<script lang="ts">
	import type { SvelteComponent } from 'svelte';

	export let title: string;
	export let desc: string;
	export let value: string;
</script>

<div class="stat">
	<div class="stat-figure text-blue-500">
		<slot />
	</div>
	<div class="stat-title">{title}</div>
	<div class="stat-value">{value}</div>
	<div class="stat-desc">{desc}</div>
</div>
