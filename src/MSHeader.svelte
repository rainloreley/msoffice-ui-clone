<script>
	import SearchIcon from './icons/SearchIcon.svelte';
</script>

<msheader>
	<headerleft>
		<svg
			class="gb_Ve self-center fill-current text-gray-600 dark:text-gray-400"
			focusable="false"
			viewBox="0 0 24 24"
			width="24"
			height="24"
		>
			<path
				d="M6,8c1.1,0 2,-0.9 2,-2s-0.9,-2 -2,-2 -2,0.9 -2,2 0.9,2 2,2zM12,20c1.1,0 2,-0.9 2,-2s-0.9,-2 -2,-2 -2,0.9 -2,2 0.9,2 2,2zM6,20c1.1,0 2,-0.9 2,-2s-0.9,-2 -2,-2 -2,0.9 -2,2 0.9,2 2,2zM6,14c1.1,0 2,-0.9 2,-2s-0.9,-2 -2,-2 -2,0.9 -2,2 0.9,2 2,2zM12,14c1.1,0 2,-0.9 2,-2s-0.9,-2 -2,-2 -2,0.9 -2,2 0.9,2 2,2zM16,6c0,1.1 0.9,2 2,2s2,-0.9 2,-2 -0.9,-2 -2,-2 -2,0.9 -2,2zM12,8c1.1,0 2,-0.9 2,-2s-0.9,-2 -2,-2 -2,0.9 -2,2 0.9,2 2,2zM18,14c1.1,0 2,-0.9 2,-2s-0.9,-2 -2,-2 -2,0.9 -2,2 0.9,2 2,2zM18,20c1.1,0 2,-0.9 2,-2s-0.9,-2 -2,-2 -2,0.9 -2,2 0.9,2 2,2z"
			/>
		</svg>
		<p>Office 365</p>
	</headerleft>
	<headercenter>
		<searchfield>
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
				class="feather feather-search searchicon"
			>
				<circle cx="11" cy="11" r="8" />
				<line x1="21" y1="21" x2="16.65" y2="16.65" />
			</svg>
			<input placeholder="Search" />
		</searchfield>
	</headercenter>
	<headerright>
		<svg
			xmlns="http://www.w3.org/2000/svg"
			width="24"
			height="24"
			viewBox="0 0 24 24"
			fill="none"
			stroke="currentColor"
			stroke-width="1"
			stroke-linecap="round"
			stroke-linejoin="round"
			class="feather feather-check-square"
			><polyline points="9 11 12 14 22 4" /><path
				d="M21 12v7a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h11"
			/></svg
		>
		<svg
			xmlns="http://www.w3.org/2000/svg"
			width="24"
			height="24"
			viewBox="0 0 24 24"
			fill="none"
			stroke="currentColor"
			strokeWidth="1"
			strokeLinecap="round"
			strokeLinejoin="round"
			class="feather feather-settings"
			><circle cx="12" cy="12" r="3" /><path
				d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1 0 2.83 2 2 0 0 1-2.83 0l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-2 2 2 2 0 0 1-2-2v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83 0 2 2 0 0 1 0-2.83l.06-.06a1.65 1.65 0 0 0 .33-1.82 1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1-2-2 2 2 0 0 1 2-2h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 0-2.83 2 2 0 0 1 2.83 0l.06.06a1.65 1.65 0 0 0 1.82.33H9a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 2-2 2 2 0 0 1 2 2v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 0 2 2 0 0 1 0 2.83l-.06.06a1.65 1.65 0 0 0-.33 1.82V9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 2 2 2 2 0 0 1-2 2h-.09a1.65 1.65 0 0 0-1.51 1z"
			/></svg
		>

		<svg
			xmlns="http://www.w3.org/2000/svg"
			width="24"
			height="24"
			viewBox="0 0 24 24"
			fill="none"
			stroke="currentColor"
			stroke-width="1"
			stroke-linecap="round"
			stroke-linejoin="round"
			class="feather feather-help-circle"
			><circle cx="12" cy="12" r="10" /><path
				d="M9.09 9a3 3 0 0 1 5.83 1c0 2-3 3-3 3"
			/><line x1="12" y1="17" x2="12.01" y2="17" /></svg
		>
		<!-- svelte-ignore a11y-img-redundant-alt -->
		<img
			class="user-pfp"
			src="https://www.gravatar.com/avatar/1615be3776f4bdfa985afdea244eb1b3"
			alt="user profile picture"
		/>
	</headerright>
</msheader>

<style>
	msheader {
		display: flex;
		justify-content: space-between;
		height: 40px;
		width: 100%;
	}

	/*headercenter {
        background-color: gray;
        border-radius: 12px;
    }*/

	headerleft {
		display: flex;
		flex-direction: row;
	}

	headerleft svg {
		align-self: center;
		margin-right: 12px;
		margin-left: 12px;
	}

	headerleft p {
		align-self: center;
	}

	.searchicon {
		align-self: center;
		color: var(--msoffice-main-color);
		margin-left: 8px;
		height: 1.2em;
		transform: scale(-1, 1);
	}

	searchfield {
		background-color: rgb(225, 223, 221);
		display: flex;
		width: 500px;
		border-radius: 5px;
		align-self: center;
		box-shadow: 2px 2px 5px 0px rgb(225, 223, 221);
	}

	searchfield input {
		border: none;
		margin: 2px;
		width: 300px;
		background-color: transparent;
	}

	headercenter {
		align-self: center;
		height: 100%;
		display: flex;
	}

	headerright {
		display: flex;
		align-self: center;
		align-items: center;
		height: 100%;
	}

	headerright .user-pfp {
		border-radius: 200px;
		width: 30px;
		height: 30px;
		margin-right: 8px;
	}

	headerright svg {
		width: 20px;
		height: 20px;
		margin-right: 24px;
	}

	headerleft p {
		color: var(--msoffice-main-color);
	}
</style>
