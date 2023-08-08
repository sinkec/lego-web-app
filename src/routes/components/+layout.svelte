<script lang="ts">
	import { AppShell } from '@skeletonlabs/skeleton';
</script>

<AppShell slotSidebarLeft="bg-surface-500/5 w-64 p-5 shadow-md">
	<svelte:fragment slot="sidebarLeft">
		<!-- Left side of NavBar -->
		<nav class="list-nav">
			<div class="mb-5">
				<h3 class="h3">Components</h3>
				<p class="text-xs">List of components used in project</p>
			</div>

			<ul>
				<li>
					<a href="/elements/lists"> Input </a>
				</li>
				<li>
					<a href="/elements/lists"> Button </a>
				</li>
				<li>
					<a href="/elements/lists"> Login </a>
				</li>
				<li>
					<a href="/elements/lists"> O nas </a>
				</li>
			</ul>
		</nav>
	</svelte:fragment>
	<svelte:fragment slot="default">
		<div class="p-5"><slot /></div>
	</svelte:fragment>
</AppShell>
