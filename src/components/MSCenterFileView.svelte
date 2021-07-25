<fileview>
	<navigationbar>
		<tabselection>
			<tabselectionitem>
				<p>All</p>
			</tabselectionitem>
			<tabselectionitem>
				<p>Last used</p>
			</tabselectionitem>
			<tabselectionitem>
				<p>Shared</p>
			</tabselectionitem>
			<tabselectionitem>
				<p class="selected">Favorites</p>
			</tabselectionitem>
		</tabselection>
		<navigationbaractions>
			<searchfield>
				<input placeholder="Type to filter the list" />
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					fill="none"
					stroke="currentColor"
					stroke-width="2"
					stroke-linecap="round"
					stroke-linejoin="round"
					class="feather feather-filter"
					><polygon points="22 3 2 3 10 12.46 10 19 14 21 14 12.46 22 3" /></svg
				>
			</searchfield>

			<uploadbutton>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					fill="none"
					stroke="currentColor"
					stroke-width="2"
					stroke-linecap="round"
					stroke-linejoin="round"
					class="feather feather-upload"
					><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4" /><polyline
						points="17 8 12 3 7 8"
					/><line x1="12" y1="3" x2="12" y2="15" /></svg
				>
				<p>Upload</p>
			</uploadbutton>
		</navigationbaractions>
	</navigationbar>
	<tableheader>
		<tableheadercontent>
			<sortbyfile>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					fill="none"
					stroke="currentColor"
					stroke-width="2"
					stroke-linecap="round"
					stroke-linejoin="round"
					class="feather feather-file"
					><path
						d="M13 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V9z"
					/><polyline points="13 2 13 9 20 9" /></svg
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
					class="feather feather-chevron-down"
					><polyline points="6 9 12 15 18 9" /></svg
				>
			</sortbyfile>
			<sortbyname>
				<p>Name</p>
			</sortbyname>
			<sortbychangedate>
				<p>Changed</p>
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
			</sortbychangedate>
			<sortbysharedby>
				<p>Shared by</p>
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
			</sortbysharedby>
			<sortbyactivity>
				<p>Activity</p>
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
			</sortbyactivity>
		</tableheadercontent>
	</tableheader>
	<fileviewcenter>
		<!-- svelte-ignore a11y-img-redundant-alt -->
		<fileviewcentermiddle>
			<div class="image" />
			<p class="title">No files saved as favories</p>
			<p class="subtitle">
				Save an element from the list as a favorite and it'll show up here.
			</p>
		</fileviewcentermiddle>
	</fileviewcenter>
</fileview>

<style>
	fileview {
		background-color: white;
		display: flex;
		flex-direction: column;
		margin-top: 32px;
		width: 100%;
	}

	navigationbar {
		display: flex;
		flex-direction: row;
		width: 100%;
		align-items: center;
		height: 60px;
		justify-content: space-between;
		margin-top: 4px;
	}

	tabselection {
		display: flex;
	}

	tabselectionitem {
		margin-left: 32px;
		color: gray;
		font-weight: 300;
		font-size: 15px;
	}

	tabselectionitem:hover p {
		font-weight: 500;
	}

	tabselectionitem .selected {
		color: black;
		font-weight: 500;
		border-bottom: 2px solid var(--msoffice-main-color);
	}

	navigationbaractions {
		display: flex;
		flex-direction: row;
		align-items: center;
	}

	searchfield {
		background-color: rgb(237, 235, 233);
		display: flex;
		align-self: center;
		align-items: center;
		padding: 2px;
	}

	searchfield svg {
		width: 17px;
		margin-right: 8px;
		color: gray;
	}

	searchfield input {
		border: none;
		margin: 0;
		width: 150px;
		margin-left: 8px;
		font-size: 12px;
		color: gray;
		background-color: transparent;
	}

	searchfield > input:focus {
		outline: none;
		border-bottom: 1px solid red !important;
	}

	searchfield input::placeholder {
		font-size: 12px;
	}

	uploadbutton {
		display: flex;
		flex-direction: row;
		color: var(--msoffice-main-color);
		font-size: 15px;
		font-weight: 400;
		align-items: center;
		margin-right: 16px;
		margin-left: 20px;
	}

	uploadbutton:hover p {
		text-decoration: underline;
	}

	uploadbutton svg {
		width: 15px;
		margin-right: 8px;
	}

	tableheader {
		border-bottom: 1px solid rgb(220, 219, 218);
		margin-left: 8px;
		margin-right: 8px;
	}

	tableheadercontent {
		margin-left: 8px;
		margin-right: 8px;
		display: flex;
		flex-direction: row;
		align-items: center;
		padding-bottom: 4px;
	}

	sortbyfile {
		height: 25px;
	}

	sortbyname {
		margin-left: 16px;
		width: 30%;
		display: flex;
		height: 25px;
		align-items: center;
		font-size: 13px;
		font-weight: 500;
	}

	sortbychangedate {
		display: flex;
		align-items: center;
		height: 25px;
		width: 20%;
		font-size: 13px;
		font-weight: 500;
	}

	sortbychangedate p {
		margin-block-start: 0;
		margin-block-end: 0;
	}

	sortbychangedate svg {
		width: 15px;
		height: 25px;
		color: gray;
		align-self: center;
	}

	sortbysharedby {
		display: flex;
		align-items: center;
		height: 25px;
		width: 20%;
		font-size: 13px;
		font-weight: 500;
	}

	sortbysharedby p {
		margin-block-start: 0;
		margin-block-end: 0;
	}

	sortbysharedby svg {
		width: 15px;
		height: 25px;
		color: gray;
		align-self: center;
	}

	sortbyactivity {
		display: flex;
		align-items: center;
		height: 25px;
		font-size: 13px;
		font-weight: 500;
	}

	sortbyactivity p {
		margin-block-start: 0;
		margin-block-end: 0;
	}

	sortbyactivity svg {
		width: 15px;
		height: 25px;
		color: gray;
		align-self: center;
	}

	sortbyfile .feather-file {
		width: 20px;
	}

	sortbyfile .feather-chevron-down {
		width: 15px;
	}

	fileviewcenter {
		width: 100%;
		display: flex;
		justify-content: center;
		margin-top: 8px;
		margin-bottom: 22px;
	}

	fileviewcentermiddle {
		text-align: center;
	}

	fileviewcentermiddle p {
		margin-block-start: 0;
		margin-block-end: 0;
		color: gray;
	}

	fileviewcentermiddle p.title {
		font-size: 22px;
		font-weight: 300;
	}

	fileviewcentermiddle p.subtitle {
		font-size: 14px;
		margin-top: 8px;
		font-weight: 300;
	}

	fileviewcentermiddle .image {
		overflow: hidden;
		box-sizing: border-box;
		direction: ltr;
		display: inline-block;
	}

	fileviewcentermiddle .image::before {
		content: url('https://officehome.cdn.office.net/images/content/images/emptystate-sprite-general-236a6305cf.png');
		left: 0;
		top: -280px;
		width: 220px;
		height: 140px;
		position: relative;
		display: block;
	}
</style>
