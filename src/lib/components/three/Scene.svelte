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
<T.Mesh position={[0, 3, 0]} rotation.y={rotation}>
	<Assembly />
	<T.DirectionalLight position={[2, 20, -10]} />

	<!-- <T.MeshBasicMaterial /> -->
</T.Mesh>
