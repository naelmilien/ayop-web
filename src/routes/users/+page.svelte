<script lang="ts">
	import type { PageProps } from './$types';

	let { data }: PageProps = $props();

	const { users } = data;
</script>

<ul>
	{#each users as user}
		<li>{user.username}</li>
	{/each}
</ul>
