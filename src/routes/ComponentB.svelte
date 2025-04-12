<script lang="ts">
	import ComponentC from './ComponentC.svelte';

	interface Props {
		value: string;
	}

	let { value }: Props = $props();
</script>

<div class="component">
	<ComponentC {value} />
</div>
