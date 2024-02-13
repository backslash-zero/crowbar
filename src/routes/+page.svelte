<script lang="ts">
	import Scene from '$lib/components/three/Scene.svelte';
	import { Canvas } from '@threlte/core';
	function scrollIntoView({ target }: any) {
		const el = document.querySelector(target.getAttribute('href'));
		if (!el) return;
		el.scrollIntoView({
			behavior: 'smooth'
		});
	}
</script>

<main class="w-full font-goudy">
	<div class="relative w-full h-[100dvh]">
		<div class="absolute w-full h-full items-stretch">
			<Canvas>
				<Scene />
			</Canvas>
		</div>
		<div class="absolute top-0 z-10 w-full flex flex-col justify-between items-center">
			<h1 class="text-7xl md:text-9xl italic font-argent">Welcome to the Crowbar</h1>
		</div>
		<div class="absolute w-full flex items-center h-12 bottom-0 z-10">
			<a
				on:click|preventDefault={scrollIntoView}
				href="#section-1"
				class="w-full h-12 text-center font-argent italic animate-pulse">↓ scroll down ↓</a
			>
		</div>
	</div>
	<div class="w-full flex flex-col items-center px-4">
		<div class="w-full md:max-w-screen-md" id="section-1">
			<div class="font-goudy py-4 text-xl w-full flex flex-col gap-4 md:max-w-screen-lg">
				<div class="w-full aspect-video">
					<iframe
						title="Crowbar - Day 2"
						width="100%"
						height="100%"
						src="https://stream.udk-berlin.de/videos/embed/058f0488-af2f-42ab-94f8-ba8001017338?start=22m2s"
						frameborder="0"
						allowfullscreen=""
						sandbox="allow-same-origin allow-scripts allow-popups"
					></iframe>
				</div>
				<h2 class="font-argent text-5xl md:text-7xl">About</h2>
				<p>
					The Crow Bar is an interactive device tailored specifically for <strong
						class="font-argent text-lg italic"
					>
						Corvids</strong
					>, aiming to lay the ground work for further research into their sensory perception and
					cognitive abilities.
				</p>
				<p>
					The device is designed to not only facilitate in-depth study of Corvids but also to be
					user-friendly and easily replicable for widespread application.
				</p>
				<p>
					The proposed <strong class="font-argent text-lg italic">open-source</strong> design is meant
					to leverage Corvid’s remarkable curiosity and problem-solving abilities. The Design includes
					a two-step puzzle which acts as a threshold to discriminate other birds to interact with the
					device.
				</p>
			</div>
			<div class="font-goudy py-4 text-xl w-full flex flex-col gap-4 md:max-w-screen-lg">
				<h2 class="font-argent text-5xl md:text-7xl">What you'll need</h2>
				<p>The Crow Bar is conceived as a fully modular and adaptive artefact.</p>
				<ul>
					<li>Access to 1 Resin Printer</li>
					<li>Access to 1 Filament Printer</li>
					<li>Any Backboard</li>
					<li>Gecko Tape</li>
					<li><strong class="font-argent text-2xl">1</strong> Empty Bottle</li>
					<li><strong class="font-argent text-2xl">2</strong> 8x16x5 Ball Bearings</li>
					<li><strong class="font-argent text-2xl">6</strong> M6x25 Screws</li>
					<li><strong class="font-argent text-2xl">1</strong> M6x16 Screw</li>
					<li><strong class="font-argent text-2xl">7</strong> M6 Washers</li>
					<li><strong class="font-argent text-2xl">6</strong> M6 Nuts</li>
					<li><strong class="font-argent text-2xl">1</strong> M8 Nuts</li>
					<li><strong class="font-argent text-2xl">2</strong> M6xM10 Threaded Inserts</li>
				</ul>
				<p>
					You are free to leave out any unwanted parts. Although the full version is designed to
					cater specifically to corvids, leaving out the puzzle components (door, rotary system)
					results in a lovely bird feeder.
				</p>
			</div>
			<div class="font-goudy py-4 text-xl w-full flex flex-col gap-8 md:max-w-screen-lg">
				<h2 class="font-argent text-5xl md:text-7xl">Instructions</h2>

				<div>
					<h3 class="font-argent text-3xl">Step 1 - Resin print the following components:</h3>
					<ul>
						<li>Door</li>
						<li>Paddle</li>
						<li>Paddle_Axle</li>
						<li>2 x Paddle_Spacer</li>
						<li>Tube</li>
					</ul>
				</div>

				<div>
					<h3 class="font-argent text-3xl">Step 2 - Filament print the following components:</h3>
					<ul>
						<li>Crow Perch Left</li>
						<li>Crow Perch Right</li>
						<li>Bowl (Optional)</li>
					</ul>
				</div>

				<h3 class="font-argent text-3xl">
					Step 3 - Screw threaded inserts into bottom thread of tube
				</h3>
				<h3 class="font-argent text-3xl">
					Step 4 - Screw threaded inserts into door hinge hole at front of tube
				</h3>
				<h3 class="font-argent text-3xl">
					Step 5 - Attach feeding bowl to Tube using 1 washer and 1 M6x25 screw
				</h3>
				<h3 class="font-argent text-3xl">
					Step 6 - Attach door to Tube using 1 washer and 1 M6x15 screw
				</h3>
				<h3 class="font-argent text-3xl">
					Step 7 - Place Tube + Feeding bowl onto mounting plate and trace the screw hole outlines
					onto the plate
				</h3>
				<h3 class="font-argent text-3xl">Step 8 - Connect Crow Perch Left with Crow Perch Right</h3>
				<h3 class="font-argent text-3xl">
					Step 9 - Place assembled Crow Perch onto the mounting plate towards lower edge and trace
					screw hole
				</h3>
				<h3 class="font-argent text-3xl">Step 10 - Drill marked holes with 8mm drill bit</h3>
				<h3 class="font-argent text-3xl">
					Step 11 - Cut insets into mounting plate so as to ensure screw heads are flush with
					mountain board surface
				</h3>
				<h3 class="font-argent text-3xl">
					Step 12 - Attach components to the plate, with the screwheads facing to the rear
				</h3>
				<h3 class="font-argent text-3xl">
					Step 13 - Attach gecko tape to the back of the mounting plate
				</h3>
				<h3 class="font-argent text-3xl">Step 14 - Mount to your surface of choice</h3>
			</div>
			<div class="font-goudy py-4 text-xl w-full flex flex-col gap-4 md:max-w-screen-lg">
				<h2 class="font-argent text-5xl md:text-7xl">Ressources</h2>
				<div class="w-full flex flex-col md:flex-row gap-4">
					<form action="https://cloud.udk-berlin.de/s/eBD8rkEke9tDGB8">
						<input
							type="submit"
							class="w-full md:w-auto font-argent italic text-2xl px-8 py-4 border-2 border-black hover:bg-slate-100 transition-all duration-300"
							value="3D-Print Files"
						/>
					</form>
					<form action="https://stream.udk-berlin.de/a/c.meunier/video-channels">
						<input
							type="submit"
							class="w-full md:w-auto font-argent italic text-2xl px-8 py-4 border-2 border-black hover:bg-slate-100 transition-all duration-300"
							value="Live Streams"
						/>
					</form>
				</div>
			</div>

			<div class="font-goudy py-4 text-xl w-full flex flex-col gap-4 md:max-w-screen-lg">
				<h2 class="font-argent text-5xl md:text-7xl">Credits</h2>
				<p>
					The Crowbar is a project by Finnegan Hardy and Célestin Meunier, made within the context
					of the Master's program <a
						href="https://www.newpractice.net/study"
						class="font-argent text-lg italic underline underline-offset-[6px]"
						>Design & Computation</a
					>, a join program between the University of Arts Berlin and Technical University.
				</p>
			</div>
			<div class="font-goudy py-4 text-xl w-full flex flex-col gap-4 md:max-w-screen-lg">
				<h2 class="font-argent text-5xl md:text-7xl">Thanks</h2>
				<p>
					Prof. Dr. Daniel D. Hromada, Prof. Albert Lang, Friedrich Goizel, Kräri the Crow, whoever
					built stream.udk.ai
				</p>
			</div>
			<div class="font-goudy py-4 text-xl w-full flex flex-col gap-4 md:max-w-screen-lg">
				<h2 class="font-argent text-5xl md:text-7xl">Contacts</h2>
				<p>Feel free to send us questions or picture of your Crowbar at (at) celest.in</p>
			</div>
		</div>
	</div>
</main>

<style lang="postcss">
	:global(html) {
	}
</style>
