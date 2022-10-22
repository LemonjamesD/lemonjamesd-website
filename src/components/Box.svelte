<script lang="ts">
	export let float: string | undefined = undefined;
</script>

<div style="float: {float}">
	<slot />
</div>

<style lang="less">
	div {
		background: linear-gradient(
			0deg,
			rgba(182, 197, 198, 1) 0%,
			rgba(203, 215, 215, 1) 100%
		);
		box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
		border-radius: 53px;
		padding: 8px;
		margin: 4px;
	}
</style>
