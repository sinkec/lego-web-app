<script lang="ts">
	// The ordering of these imports is critical to your app working properly
	import '../theme.postcss';
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Most of your app wide CSS should be put in this file
	import '../app.postcss';
	import { AppShell, AppBar, LightSwitch } from '@skeletonlabs/skeleton';

	//assets imports
	import logo from '$lib/assets/logo.svg';
</script>

<!-- App Shell -->
<AppShell>
	<svelte:fragment slot="header">
		<!-- App Bar -->
		<AppBar
			shadow="shadow-md"
			gridColumns="grid-cols-3"
			slotLead="place-self-start font-semibold space-x-5"
			slotDefault="place-self-center"
			slotTrail="place-content-end"
		>
			<svelte:fragment slot="lead">
				<!-- Left side of NavBar -->
				<img class="logo" src={logo} alt="logo" />
				<span>brihtnabuča</span>
			</svelte:fragment>

			<svelte:fragment slot="default">
				<!-- Center of NavBar -->
				<nav>
					<ul class="flex space-x-10 font-semibold">
						<li>
							<a href="/elements/lists">
								<span class="flex-auto">Domov</span>
							</a>
						</li>
						<li>
							<a href="/elements/lists">
								<span class="flex-auto">Ponudba</span>
							</a>
						</li>
						<li>
							<a href="/elements/lists">
								<span class="flex-auto">Delavnica</span>
							</a>
						</li>
						<li>
							<a href="/elements/lists">
								<span class="flex-auto whitespace-nowrap">O nas</span>
							</a>
						</li>
					</ul>
				</nav>
			</svelte:fragment>

			<svelte:fragment slot="trail">
				<!-- Right side of NavBar -->
				<LightSwitch />
			</svelte:fragment>
		</AppBar>
	</svelte:fragment>
	<!-- Page Route Content -->
	<slot />
</AppShell>
