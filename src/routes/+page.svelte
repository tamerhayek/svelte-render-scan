<script lang="ts">
	import { RenderScan } from 'svelte-render-scan';
	import '../app.css';
	import ComponentA from './ComponentA.svelte';

	let value = $state('svelte');
</script>

<svelte:head>
	<title>Svelte render scan</title>
	<meta name="description" content="Svelte render scan" />
</svelte:head>

<RenderScan />

<div class="container">
	<h1>Svelte render scan</h1>

	<a href="https://github.com/tamerhayek/svelte-render-scan" target="_blank" rel="noreferrer">
		Github repository
	</a>

	<div class="form">
		<label for="value">Modifica il testo:</label>
		<input id="value" type="text" bind:value />
	</div>

	<div class="component">
		<ComponentA {value} />
	</div>
</div>
