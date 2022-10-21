<script lang="ts">
</script>

<div>
	<slot />
</div>

<style lang="less">
	@to: #dadada;

	div {
		background-color: @to;
		box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
		border-radius: 53px;
		padding: 8px;
	}
</style>
