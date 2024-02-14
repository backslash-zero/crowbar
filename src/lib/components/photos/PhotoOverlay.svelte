<script lang="ts">
	import { XIcon } from 'svelte-feather-icons';
	export let pictureURL: string = '';
</script>

<div class="relative w-full max-w-80 rounded-lg bg-slate-500/50 p-4 shadow-sm backdrop-blur-sm">
	<img class="round-md" src={pictureURL} alt="" />
	<XIcon class="absolute w-8 top-2 right-2" on:click></XIcon>
</div>
