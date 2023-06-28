<script>
	import { browser } from '$app/environment';
	import { page } from '$app/stores';
	import '../app.css';

	/** @type {import('./$types').LayoutServerData} */
	export let data;
</script>

<div class="app bg-slate-200 text-pink-500">
	<main>
		<slot />
	</main>

	<footer>
		<p>developed by www.solidstack.io</p>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
