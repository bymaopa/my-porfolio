<script lang="ts">

	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<meta charset="utf-8" />
	<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
	<link rel="icon" href={favicon} />
	<title>&gt; Mi Porfolio</title>
	
</svelte:head>

{@render children()}
