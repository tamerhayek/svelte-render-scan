<script lang="ts">
	import ComponentD from './ComponentD.svelte';

	interface Props {
		value: string;
	}

	let { value }: Props = $props();
</script>

<div class="component">
	<ComponentD {value} />
</div>
