<script>
	import { T, useTask } from '@threlte/core';
	import { interactivity } from '@threlte/extras';
	import { OrbitControls } from '@threlte/extras';
	import Assembly from './Assembly.svelte';

	interactivity();
	let rotation = Math.PI;
	useTask((delta) => {
		rotation += delta / 5;
	});
</script>

<T.PerspectiveCamera
	makeDefault
	position={[10, 0, 10]}
	on:create={({ ref }) => {
		ref.lookAt(0, 0, 0);
	}}
>
	<OrbitControls />
</T.PerspectiveCamera>
<T.DirectionalLight position={[20, 20, 20]} castShadow />
<T.Mesh position={[0, 3, 0]} rotation.y={rotation} castShadow>
	<Assembly />

	<!-- <T.MeshBasicMaterial /> -->
</T.Mesh>
