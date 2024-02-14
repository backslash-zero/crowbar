<script lang="ts">
	import { EyeIcon } from 'svelte-feather-icons';
	import PhotoOverlay from './PhotoOverlay.svelte';
	let isPhotoVisible = false;

	function togglePhotoVisibility() {
		isPhotoVisible = !isPhotoVisible;
	}

	export let pictureURL: string = '';
</script>

<button
	on:click={togglePhotoVisibility}
	class="cursor-pointer hover:opacity-50 transition-all duration-300"
>
	<EyeIcon />
</button>
{#if isPhotoVisible}
	<PhotoOverlay {pictureURL} on:click={togglePhotoVisibility} />
{/if}
