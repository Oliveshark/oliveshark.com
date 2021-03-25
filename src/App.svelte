<script lang="ts">
	import ContactItem from './ContactItem.svelte';

	const contactEntries: any[] = [
		{
			link: "https://twitter.com/LiquidityC",
			label: "Twitter",
			icon: "fab fa-twitter",
		},
		{
			link: "https://github.com/LiquidityC",
			label: "GitHub",
			icon: "fab fa-github",
		},
		{
			link: "https://www.linkedin.com/in/linus-probert/",
			label: "LinkedIn",
			icon: "fab fa-linkedin",
		},
		{
			link: "https://store.steampowered.com/curator/33516566-Oliveshark/",
			label: "Steam",
			icon: "fab fa-steam",
		},
	];
</script>

<main>
	<div>
		<img alt="Oliveshark Logo" src="logo.png">
	</div>
	<div>
		{#each contactEntries as entry}
			<ContactItem {...entry}/>
		{/each}
	</div>
</main>

<style lang="scss">
	:global(body) {
		background-color: #639bff;
	}

	main {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}
</style>
