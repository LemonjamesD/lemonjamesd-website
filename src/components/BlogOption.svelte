<script lang="ts">
	import BoxNav from "./BoxNav.svelte";

	export let page: string;
	export let title: string;
	export let date: string;
</script>

<BoxNav {page}>
	<center><h1>{title}</h1></center>
	<center><h5>{"Date Created: " + date}</h5></center>
	<center><slot /></center>
	<br />
</BoxNav>

<style lang="less">
	center {
		align-items: center;
		align-content: center;
	}
</style>
