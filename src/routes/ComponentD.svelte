<script lang="ts">
	interface Props {
		value: string;
	}

	let { value }: Props = $props();
</script>

<div class="component">
	<p>{value}</p>
</div>
