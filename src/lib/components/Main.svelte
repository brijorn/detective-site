<script>
	import Status from './Status/index.svelte';
	import Tab from './Tab.svelte';
	import { Info, History  } from 'lucide-svelte';
</script>

<div class="flex flex-row items-center justify-center gap-10">
	<Tab name="About" Icon={Info} index={0} />
	<Status />
	<Tab name="Logs" Icon={History} index={1} />
</div>
