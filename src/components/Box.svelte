<script lang="ts">
	export let float: string | undefined = undefined;
	export let className: string | undefined = undefined;
</script>

<div class={className} style="float: {float}">
	<slot />
</div>

<style lang="less">
	@from: rgb(182, 197, 198);
	@to: rgb(203, 215, 215);

	div {
		background: linear-gradient(0deg, @from 0%, @to 100%);
		box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
		border-radius: 53px;
		padding: 8px;
		margin: 4px;
	}
</style>
