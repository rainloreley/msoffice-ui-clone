<script>
	import MSHeader from './MSHeader.svelte';
	import MSSidebar from './MSSidebar.svelte';
	import MSCenterView from './MSCenterView.svelte';
</script>

<main>
	<MSHeader />
	<mainbody>
		<MSSidebar />
		<MSCenterView />
	</mainbody>
</main>

<!--<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>-->
<style>
	:root {
		--msoffice-main-color: rgb(213, 58, 2);
	}

	:global(body) {
		padding: 0;
		background-color: rgb(250, 249, 248);
		position: fixed;
		scrollbar-width: none;
	}

	:global(body::-webkit-scrollbar) {
		width: 0;
		height: 0;
		display: none;
	}

	main {
		width: 100%;
		height: 100%;
		margin: 0 auto;
	}
	mainbody {
		display: flex;
		flex-direction: row;
		height: calc(100% - 40px);
		scrollbar-width: 0;
	}

	mainbody::-webkit-scrollbar {
		width: 0;
		display: none;
		height: 0;
	}
</style>
