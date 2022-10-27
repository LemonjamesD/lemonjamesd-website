<script lang="ts">
	export let rotation = 0;

	function cssVariables(node: HTMLElement, variables: Object) {
		setCssVariables(node, variables);

		return {
			update(variables: Array<string>) {
				setCssVariables(node, variables);
			},
		};
	}
	function setCssVariables(node: HTMLElement, variables: any) {
		for (const name in variables) {
			node.style.setProperty(`--${name}`, variables[name]);
		}
	}
</script>

<div use:cssVariables={{ rotation }}>
	<p>
		<slot />
	</p>
</div>

<style lang="less">
	div {
		transform: rotate(calc(var(--rotation) * 1deg));

		background-color: rgb(204, 255, 255);

		border-radius: 32px;
		padding: 1px;

		width: fit-content;
	}

	p {
		padding: 8px;

		background-color: rgb(165, 213, 224);

		border-radius: 16px;
		margin: 8px;

		width: fit-content;
	}
</style>
