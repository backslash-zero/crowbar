<!--
Auto-generated by: https://github.com/threlte/threlte/tree/main/packages/gltf
Command: npx @threlte/gltf@2.0.1 ../Assembly.glb
-->

<script>
	import { Group, MeshStandardMaterial } from 'three';
	import { T, forwardEventHandlers } from '@threlte/core';
	import { useGltf } from '@threlte/extras';

	export const ref = new Group();

	const gltf = useGltf('/assets/Assembly.glb');

	const component = forwardEventHandlers();
</script>

<T is={ref} dispose={false} {...$$restProps} bind:this={$component}>
	{#await gltf}
		<slot name="fallback" />
	{:then gltf}
		<T.Mesh geometry={gltf.nodes.imagetostl_mesh0.geometry} scale={40} receiveShadow>
			<T.MeshStandardMaterial color="#ffffff" receiveShadow />
		</T.Mesh>
	{:catch error}
		<slot name="error" {error} />
	{/await}

	<slot {ref} />
</T>
