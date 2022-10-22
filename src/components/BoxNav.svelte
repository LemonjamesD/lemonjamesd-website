<script lang="ts">
	import Box from "./Box.svelte";
	export let page = "/";
</script>

<a href={page}>
	<Box float="left"><slot /></Box>
</a>
