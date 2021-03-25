<script lang="ts">
	export let link: string;
	export let label: string;
	export let icon: string;
</script>

<span class="item">
	<a href={link}>
		<i class={icon}></i> {label}
	</a>
</span>

<style lang="scss">
	.item {
		display: inline-block;
		margin-left: 1rem;
	}
	a {
		text-decoration: none;
		color: black;

		&:visited {
			text-decoration: none;
			color: black;
		}
	}
</style>
