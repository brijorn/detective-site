<script lang="ts">
import Avatar from "./Avatar.svelte";
import Game from "./Game.svelte";
import Name from "./Name.svelte";


    const status = "Online";

    const statusColor = () => {
        if (status == "Online") return "shadow-green-200"

        return "shadow-gray-500"
    }
</script>

<div
	class={`flex flex-row gap-2 rounded-full m-5 p-5 shadow-lg items-center justify-center ${statusColor()}`}
>
	<Avatar />
	<div class="flex flex-col">
		<Name />
		<p >Volos is now playing <span class="text-green-500 hover:text-green-600 transition-all">A One Piece Game</span></p>
	</div>

</div>
