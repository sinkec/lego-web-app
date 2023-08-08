<script lang="ts">
	export let type: 'button' | 'submit' | 'reset' = 'button';
	export let onClick = () => {};
	export let style: 'primary' | 'secondary' | 'testing' = 'primary';

	let styleClasses = {
		primary: 'btn btn-lg variant-filled-primary',
		secondary: 'btn btn-sm variant-filled-secondary',
		testing: 'btn btn-lg variant-filled-error'
	};

	console.log(styleClasses[style]);
	let customClass = styleClasses[style];
</script>

<button {type} on:click={onClick} class={customClass}> <slot /></button>
