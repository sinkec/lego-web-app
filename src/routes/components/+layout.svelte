<script lang="ts">
	import { AppShell } from '@skeletonlabs/skeleton';
</script>

<AppShell slotSidebarLeft="p-5 card rounded-none shadow-lg">
	<svelte:fragment slot="sidebarLeft">
		<!-- Left side of NavBar -->
		<nav class="list-nav">
			<div class="mb-5">
				<h3 class="h3">Components</h3>
				<p class="text-xs">List of components used in project</p>
			</div>

			<ul>
				<li>
					<a href="/components/input"> Input </a>
				</li>
				<li>
					<a href="/components/button"> Button </a>
				</li>
				<li>
					<a href="/components/login"> Login </a>
				</li>
				<li>
					<a href="/components/library"> Library </a>
				</li>
			</ul>
		</nav>
	</svelte:fragment>
	<svelte:fragment slot="default">
		<div class="card flex mx-10 my-5 px-5 py-5"><slot /></div>
	</svelte:fragment>
</AppShell>
