<script lang="ts">
	export let value: string = "Default";
	export let disabled: boolean = false;
	export let variant: string = "";
	export let size: string = "";
	export let disableShadow: boolean = false;
	export let color: string = "default";
	export let startIcon: string = "";
	export let endIcon: string = "";
</script>

<button
	class:text={variant === "text"}
	class:outline={variant === "outline"}
	class:sm={size === "sm"}
	class:md={size === "md" || size === ""}
	class:lg={size === "lg"}
	class:disableShadow={disableShadow || disabled || variant != "text"}
	class:defaultColor={variant === ""
						&& (color === "default"
							|| (color != "primary" && color != "secondary"))}
	class:primaryColor={color === "primary"
						|| disableShadow
						|| size != ""
						|| startIcon != ""
						|| endIcon != ""}
	class:secondaryColor={color === "secondary"}
	class:dangerColor={color === "danger"}
	class:disable={disabled}

	disabled='{disabled}'
>
	{#if startIcon != ""}
		<span class="material-icons paddingRight">
			{startIcon}
		</span>
	{/if}
			{value}
	{#if endIcon != ""}
		<span class="material-icons paddingLeft">
			{endIcon}
		</span>
	{/if}
</button>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Noto Sans JP:wght@500&display=swap');

	.material-icons {
		font-size: 14px;
		line-height: 18px;
	}

	.paddingLeft {
		padding-left: 8px;
	}

	.paddingRight {
		padding-right: 8px;
	}

	button {
		font-family: 'Noto Sans JP';
		font-style: normal;
		font-weight: 500;
		font-size: 14px;
		line-height: 20px;
		text-align: center;
		box-shadow: 0px 2px 3px rgba(51, 51, 51, 0.2);
		border-radius: 6px;
		border: none;
		cursor: pointer;
	}

	button:hover, button:focus {
		box-shadow: 0px 2px 3px rgba(51, 51, 51, 0.2);
		border-radius: 6px;
	}

	.disableShadow, .disableShadow:hover, .disableShadow:focus {
		box-shadow: none;
	}

	.outline {
		color: #3D5AFE;
		border: 1px solid #3D5AFE;
		background: white;
	}

	.outline:hover, .outline:focus {
		background: rgba(41, 98, 255, 0.1);
	}

	.text {
		padding: 0;
		background: transparent !important;
		box-shadow: none;
		color: #3D5AFE;
	}

	.text:hover, .text:focus {
		background: rgba(41, 98, 255, 0.1) !important;
		border-radius: 6px;
		box-shadow: none;
	}

	.sm {
		padding: 4px 9px;
	}

	.md {
		padding: 8px 18px;
	}

	.lg {
		padding: 10px 22px;
	}

	.defaultColor {
		color: #3F3F3F;
		background: #E0E0E0;
	}

	.defaultColor:hover, .defaultColor:focus {
		background: #AEAEAE;
	}

	.primaryColor {
		color: white;
		background: #2962FF;
	}

	.primaryColor:hover, .primaryColor:focus {
		background: #0039CB;
	}

	.secondaryColor {
		color: white;
		background: #455A64;
	}

	.secondaryColor:hover, .secondaryColor:focus {
		background: #1C313A;
	}

	.dangerColor {
		color: white;
		background: #D32F2F;;
	}

	.dangerColor:hover, .dangerColor:focus {
		background: #9A0007;
	}

	.disable {
		color: #9E9E9E;
		background: #E0E0E0;
	}
</style>
