<script>
	import Scene from '$lib/components/three/Scene.svelte';
	import { Canvas } from '@threlte/core';
</script>

<main class="w-full font-goudy">
	<div class="relative w-full h-[100dvh]">
		<div class="absolute w-full h-full items-stretch">
			<Canvas>
				<Scene />
			</Canvas>
		</div>
		<div class="absolute top-0 z-10 w-full flex flex-col justify-between items-center">
			<h1 class="text-7xl italic font-argent">Welcome to the Crowbar</h1>
		</div>
		<div class="absolute bottom-0 z-10 w-full">
			<p class="w-full h-12 text-center font-argent italic animate-pulse">↓ scroll down ↓</p>
		</div>
	</div>
	<div class="font-goudy py-4 text-xl w-full flex flex-col gap-4 md:max-w-screen-lg">
		<h2 class="font-argent text-7xl">About</h2>
		<p>
			The Crow Bar is interactive device tailored specifically to Corvids, aiming to lay the ground
			work for further research into their sensory perception and cognitive abilities.
		</p>
		<p>
			The device is designed to not only facilitate in-depth study of Corvids but also to be
			user-friendly and easily replicable for widespread application.
		</p>
		<p>
			The propose open-source design is meant to leverage Corvid’s remarkable curiosity and
			problem-solving abilities. The Design includes a two-step puzzle which acts as a threshold to
			discriminate other birds to interact with the device.
		</p>
	</div>
	<div class="font-goudy py-4 text-xl w-full flex flex-col gap-4 md:max-w-screen-lg">
		<h2 class="font-argent text-7xl">How to</h2>
		<p>blablabla</p>
	</div>
	<div class="font-goudy py-4 text-xl w-full flex flex-col gap-4 md:max-w-screen-lg">
		<h2 class="font-argent text-7xl">Files</h2>
		<p>file 1</p>
		<p>file 2</p>
		<p>file 3</p>
	</div>
	<div class="font-goudy py-4 text-xl w-full flex flex-col gap-4 md:max-w-screen-lg">
		<h2 class="font-argent text-7xl">Credits</h2>
		<p>
			The Crowbar is a project by Finnegan Hardy and Célestin Meunier, made within the context of
			the master's program Design & Computation, a join program between the University of Arts
			Berlin and Technical University.
		</p>
		<p>
			Thanks to everyone who helped on this project: Prof. Dr. Daniel D. Hromada for both his
			technical support and his beautiful outlook on technology and every life forms
		</p>
		<p>
			Everyone at <a
				href="https://www.newpractice.net/study"
				class="font-argent text-lg italic underline underline-offset-[6px]">Design & Computation</a
			>
		</p>
	</div>
	<div class="font-goudy py-4 text-xl w-full flex flex-col gap-4 md:max-w-screen-lg">
		<h2 class="font-argent text-7xl">Contacts</h2>
		<p>hello (at) celest.in</p>
	</div>
</main>

<style lang="postcss">
	:global(html) {
	}
</style>
