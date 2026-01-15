<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon-16x16.png';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<main class="min-h-screen bg-base-200 text-base-content">
	{@render children()}
</main>
