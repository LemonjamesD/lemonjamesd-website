<script lang="ts">
	import Box from "./Box.svelte";
	export let page = "/";
	export let className: string | undefined = undefined;
</script>

<a href={page}>
	<Box {className} float="left"><slot /></Box>
</a>
