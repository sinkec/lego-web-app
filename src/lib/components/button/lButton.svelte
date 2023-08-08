<script lang="ts">
	export let type: 'button' | 'submit' | 'reset' = 'button';
	export let onClick = () => {};
	export let style: 'primary' | 'secondary' | 'error' | 'warning' | 'success' | 'lighter' | 'icon' = 'primary';

	let styleClasses = {
		primary: 'btn btn-lg variant-filled-primary',
		secondary: 'btn btn-sm variant-filled-secondary',
		error: 'btn btn-lg variant-filled-error',
		warning: 'btn btn-lg variant-filled-warning',
		success: 'btn btn-lg variant-filled-success',
		lighter: 'btn btn-lg variant-soft-surface',
		icon: 'btn-icon btn-icon-xl variant-filled'
	};

	console.log(styleClasses[style]);
	let customClass = styleClasses[style];
</script>

<button type={type} on:click={onClick} class={customClass}> <slot /></button>

<button class="btn text-"></button>

<!-- submit gumb, primary gumb, normaln gumb (malo svetlejše kot ozadje), outline gumb (warning, success, error -- rdec - error, zelen, rumen) -->


<style lang="postcss">
	.variant-filled-error {
	@apply font-bold;
	}
</style>