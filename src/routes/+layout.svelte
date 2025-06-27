<script lang="ts">
	import '../app.css';
	// Supports weights 200-700
	import '@fontsource-variable/oswald';
	import '@fontsource/source-sans-pro';

	let { children } = $props();
</script>

<svelte:head>
	<title>Practically Cool</title>
</svelte:head>

{@render children()}
