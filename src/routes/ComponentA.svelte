<script lang="ts">
	import ComponentB from './ComponentB.svelte';

	interface Props {
		value: string;
	}

	let { value }: Props = $props();
</script>

<div class="component">
	<ComponentB {value} />
</div>
