<script>
	export let openingdate;
	export let imageurl;
	export let filename;
	export let fileurl;
</script>

<outerframe>
	<upperrow>
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
			class="feather feather-folder"
			><path
				d="M22 19a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h5l2 3h9a2 2 0 0 1 2 2z"
			/></svg
		>
		<div>
			<p>You recently opened this file.</p>
			<p>{openingdate}</p>
		</div>
	</upperrow>
	<img src={imageurl} alt="" />
	<lowerrow>
		<p class="filename">{filename}</p>
		<p class="fileurl">{fileurl}</p>
	</lowerrow>
</outerframe>

<style>
	outerframe {
		background-color: white;
		display: flex;
		flex-direction: column;
		padding: 8px;
		max-width: 250px;
		margin-right: 16px;
		box-shadow: 1px 1px 5px 0px rgb(225, 223, 221);
	}

	img {
		width: 100%;
		height: 75%;
	}

	upperrow {
		display: flex;
		flex-direction: row;
		align-items: center;
		margin: 8px 8px 16px 8px;
	}
	upperrow svg {
		color: var(--msoffice-main-color);
		width: 20px;
	}
	upperrow div p {
		margin-left: 8px;
		margin-block-start: 0;
		color: gray;
		font-size: 14px;
		margin-block-end: 0;
	}

	lowerrow p {
		margin-block-start: 0;
		margin-block-end: 0;
		margin-left: 8px;
		margin-right: 8px;
	}

	lowerrow .filename {
		margin-top: 12px;
	}

	lowerrow .fileurl {
		overflow: hidden;
		color: gray;
		margin-top: 4px;
		font-size: 12px;
		text-overflow: ellipsis;
		white-space: nowrap;
	}
</style>
