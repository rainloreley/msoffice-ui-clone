<script>
	import MSCenterViewRecommendedCell from './components/MSCenterViewRecommendedCell.svelte';
	import MSCenterFileView from './components/MSCenterFileView.svelte';
</script>

<mscenterview>
	<innerview>
		<titleview>
			<p class="greeting">Good morning!</p>
			<installofficebutton>
				<p>Install Office</p>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					fill="none"
					stroke="currentColor"
					stroke-width="1.5"
					stroke-linecap="round"
					stroke-linejoin="round"
					class="feather feather-chevron-down"
					><polyline points="6 9 12 15 18 9" /></svg
				>
			</installofficebutton>
		</titleview>
		<recommendedview>
			<recommendedviewline>
				<p>Recommended</p>
				<navigationbuttons>
					<svg
						xmlns="http://www.w3.org/2000/svg"
						width="24"
						height="24"
						viewBox="0 0 24 24"
						fill="none"
						stroke="currentColor"
						stroke-width="1.5"
						stroke-linecap="round"
						stroke-linejoin="round"
						class="feather feather-chevron-left"
						><polyline points="15 18 9 12 15 6" /></svg
					>
					<svg
						xmlns="http://www.w3.org/2000/svg"
						width="24"
						height="24"
						viewBox="0 0 24 24"
						fill="none"
						stroke="currentColor"
						stroke-width="1.5"
						stroke-linecap="round"
						stroke-linejoin="round"
						class="feather feather-chevron-right"
						><polyline points="9 18 15 12 9 6" /></svg
					>
				</navigationbuttons>
			</recommendedviewline>
			<recommendedviewframes>
				<MSCenterViewRecommendedCell
					openingdate="Thursday at 3:51pm"
					imageurl="https://images.unsplash.com/photo-1463947628408-f8581a2f4aca?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
					filename="beautiful sky"
					fileurl="https://unsplash.com/photos/PEm_sLmJT-w"
				/>

				<MSCenterViewRecommendedCell
					openingdate="Monday at 2:19pm"
					imageurl="https://images.unsplash.com/photo-1534214526114-0ea4d47b04f2?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
					filename="Akabane, Kita, Japan"
					fileurl="https://unsplash.com/photos/5-GNa303REg"
				/>

				<MSCenterViewRecommendedCell
					openingdate="Tuesday at 5:10am"
					imageurl="https://images.unsplash.com/photo-1501973801540-537f08ccae7b?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
					filename="Last October"
					fileurl="https://unsplash.com/photos/uuBBew6g2jM"
				/>
			</recommendedviewframes>
		</recommendedview>
		<MSCenterFileView />
	</innerview>
</mscenterview>

<style>
	mscenterview {
		width: 100%;
		display: flex;
		justify-content: center;
	}
	innerview {
		display: flex;
		flex-direction: column;
		width: 70%;
	}

	titleview {
		width: 100%;
		padding-top: 40px;
		height: 50px;
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: space-between;
	}

	titleview .greeting {
		font-weight: 500;
		font-size: x-large;
	}

	recommendedview {
		display: flex;
		flex-direction: column;
	}

	recommendedviewline {
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: space-between;
	}

	recommendedviewline p {
		font-size: 16px;
		font-weight: 500;
	}

	recommendedviewframes {
		display: flex;
		flex-direction: row;
	}

	navigationbuttons svg.feather-chevron-left {
		color: lightgray;
		margin-right: 8px;
	}

	navigationbuttons svg.feather-chevron-right {
		color: gray;
	}

	installofficebutton {
		display: flex;
		flex-direction: row;
		align-items: center;
		color: var(--msoffice-main-color);
		padding: 0px 16px 0px 16px;
		background-color: white;
		box-shadow: 1px 1px 5px 0px rgb(225, 223, 221);
	}

	installofficebutton:hover {
		background-color: var(--msoffice-main-color);
	}

	installofficebutton p {
		font-size: 13px;
		font-weight: 500;
		margin-right: 6px;
		margin-block-start: 10px;
		margin-block-end: 10px;
	}

	installofficebutton:hover p {
		color: white;
	}

	installofficebutton:hover svg {
		color: white;
	}

	installofficebutton svg {
		width: 18px;
	}
</style>
