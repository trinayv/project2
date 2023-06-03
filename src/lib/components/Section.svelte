<script lang="ts">
	import Icon from 'svelte-awesome';
	import type { IconType } from 'svelte-awesome/components/Icon.svelte';

	export let iconData: IconType;
	export let title: string;
</script>

<div class="container">
	<div class="section-title">
		<Icon data={iconData} />
		{title}
	</div>
	<slot />
</div>

<style>
	.section-title {
      display: flex;
	  align-items: center;
	  gap: 12px;
	  font-weight: 500;
      font-family: "Nunito Sans", sans-serif;
}
	.container {
		display: flex;
		flex-direction: column;
        gap: 16px;

	}


</style>
