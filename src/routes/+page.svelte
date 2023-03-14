<script>
	import TitleName from '../components/TitleName.svelte';
</script>

<div class="name-container">
	<TitleName />
</div>

<style lang="postcss">
	.name-container {
		display: flex;
		margin: clamp(1rem, 15vw - 3rem, 4rem) auto;
		justify-content: center;
		height: clamp(50px, 30px + 20vw, 112px);
		@apply lg:h-28 lg:w-auto;
	}
</style>
