<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<title>eSafety Guidebook</title>
	<link rel="icon" href={favicon} />
</svelte:head>

<main>
	<div class="content">
		{@render children()}
	</div>
</main>
