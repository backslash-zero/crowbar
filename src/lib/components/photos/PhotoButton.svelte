<script lang="ts">
	import { EyeIcon } from 'svelte-feather-icons';
	import PhotoOverlay from './PhotoOverlay.svelte';
	let isPhotoVisible = false;

	function togglePhotoVisibility() {
		isPhotoVisible = !isPhotoVisible;
	}

	export let pictureURL: string = '';
</script>

<span on:click={togglePhotoVisibility}>
	<EyeIcon />
</span>
<PhotoOverlay {pictureURL} on:clik={togglePhotoVisibility} />
