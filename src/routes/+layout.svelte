<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';
	import MyHeader from '$lib/components/header.svelte'

	let { children } = $props();
</script>

<svelte:head>
	<title>eSafety Guidebook</title>
	<link rel="icon" href={favicon} />
</svelte:head>

<MyHeader />

<main>
	<div class="content">
		{@render children()}
	</div>
</main>
