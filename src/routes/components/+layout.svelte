<script lang="ts">
	import { AppShell } from '@skeletonlabs/skeleton';
</script>

<AppShell slotSidebarLeft="bg-surface-500/5 w-64 p-5">
	<svelte:fragment slot="sidebarLeft">
		<!-- Left side of NavBar -->
		<nav class="list-nav">
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
</AppShell>
