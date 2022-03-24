<script lang="ts">
	import '../app.css';
</script>

<div class="flex flex-col p-4  w-full max-w-5xl mx-auto  prose md:prose-lg lg:prose-xl">
	<header />

	<main>
		<slot />
	</main>

	<footer class="flex flex-col justify-center items-center p-10">
		<p>
			visit <a class="font-bold" href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit
		</p>
	</footer>
</div>
