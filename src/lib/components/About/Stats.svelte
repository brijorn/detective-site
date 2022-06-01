<script lang="ts">
	import { Timer, Play, Undo2 } from 'lucide-svelte';
	import Stat from './Stat.svelte';
</script>

<div class="stats shadow">
	<Stat title="Time Spent" desc="Started Today at 8:35 PM" value="3h 15min"><Timer /></Stat>

	<Stat title="Last Played" desc="Last time the game was played" value="Today at 11:48pm"
		><Undo2 /></Stat
	>

	<Stat
		title="Total Time Played"
		desc="Total amount of time you have played this game"
		value="50 hours"><Play /></Stat
	>
</div>
