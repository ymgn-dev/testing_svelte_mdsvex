# How to setup

1. npm init svelte@next my-app
2. npx svelte-add tailwindcss
3. npx svelte-add mdsvex
4. pnpm install -D @tailwindcss/typography
5. 
In tailwind.config.js:

```
module.exports = {
  theme: {
    // ...
  },
  plugins: [
+   require('@tailwindcss/typography'),
    // ...
  ],
}
```

6. Modify __layout.svelte as follows

```
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

```