<script lang="ts">
	import '../reset.css';
</script>

<div class="app-container">
	<header>
	</header>
	<main></main>
	<footer>
		<p>Made by Stel Clementine 🎀</p>
	</footer>
</div>

<style lang="scss">
	@use 'sass:color';
	@use 'sass:math';
	@function rem($pxValue) {
		@return math.div($pxValue, 16px) * 1rem;
	}
	.app-container {
		display: flex;
		flex-direction: column;
		height: 100vh;
	}
	header {
		flex: 0 1 auto;
		display: flex;
		flex-direction: column;
		align-items: center;
	}
	main {
		flex: 1 1 auto;
	}
	footer {
		flex: 0 0 auto;
		display: flex;
		justify-content: center;
		padding: rem(6px);
		background: rgba(0, 0, 0, 0.5);
		color: white;
	}
	}
</style>
