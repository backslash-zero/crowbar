<script lang="ts">
	import { XIcon } from 'svelte-feather-icons';
	export let pictureURL: string = '';
</script>

<div class="fixed inset-0 flex items-center justify-center">
	<div class="w-full max-w-64 rounded-lg bg-slate-200/50 p-2 shadow-sm backdrop-blur-sm">
		<img class="rounded-md" src={pictureURL} alt="" />
		<button on:click class="absolute z-10 w-10 h-10 top-2 right-0 text-white cursor-pointer">
			<XIcon class=""></XIcon>
		</button>
	</div>
</div>
