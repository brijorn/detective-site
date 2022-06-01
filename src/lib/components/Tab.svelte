<script lang="ts">
	import { selectedTab } from '$lib/store';
	export let name: string;
	export let Icon: any;
	export let index: number;



	let baseStyle =
		'tab border-b-2 grid grid-cols-2 hover:border-b-4 transition-all hover:border-blue-300 hover:text-blue-300';
	let style = baseStyle;
	let activeStyle = ' text-blue-500 border-blue-500 border-b-4';
    selectedTab.subscribe((v) => {
		if (v == index) style = baseStyle + activeStyle;
		else style = baseStyle;
	});
	function handleClick() {
		console.log('click');
		selectedTab.set(index);
	}
</script>

<div on:click={handleClick} class={style}>
	<Icon class="h-5 w-5" />
	{name}
</div>
