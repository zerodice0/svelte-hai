<script>
	import AccountBoxIcon from 'svelte-material-icons/AccountBox.svelte'
	import KeyIcon from 'svelte-material-icons/Key.svelte'
	const login = () => {
		alert("hello");
	}
</script>

<main>
	<div class="simple-modal">
		<div class="header">
			<span class="title">HAT</span>
			<span class='subtitle'>How about this?</span>
		</div>
		<div class="body">
			<div class="icon-input">
				<div class="icon">
					<AccountBoxIcon size={"2rem"}/>
				</div>
				<input type="text"
					placeholder="login id"/>
			</div>
			
			<div class="icon-input">
				<div class="icon">
					<KeyIcon size={"2em"}/>
				</div>
				<input type="text"
					placeholder="password"/>
			</div>
			<button on:click="{login}">
				Login
			</button>
		</div>
	</div>
</main>

<style lang="scss">
	main {
		width: 100%;
		height: 100%;
		display:flex;
		justify-content: center;
		flex-direction: row;
		align-content: center;
		align-items: center;
		
		.simple-modal {
			display: flexbox;
			width: 20rem;
			border-radius: 7px;
			padding: 7px;
			background: #ededed;
			box-shadow: inset 14px 14px 28px #afafaf,
            inset -14px -14px 28px #ffffff;
			display: flexbox;
			flex-direction: column;

			.header {
				display:flex;
				justify-content: center;
				flex-direction: column;
				width: 100%;
				text-align: center;
				padding-top: 1rem;
				padding-bottom: 1rem;
				text-shadow:  4px 4px 6px #afafaf,
										-4px -4px 6px #ffffff;

				.title {
					font-size: 1.5rem;
				}
			}

			.body {
				display: flex;
				flex-direction: column;
				justify-content: center;
				border-radius: 5px;
				background: #ffffff;
				box-shadow:  3px 3px 12px #afafaf,
										-3px -3px 12px #ffffff;
				margin-left: 1rem;
				margin-right: 1rem;
				margin-bottom: 1rem;
				padding-top: 1rem;
				padding-bottom: 1rem;

				input, button {
					margin: 0.5rem 1rem 0.5rem 1rem;
				}

				.icon-input {
					display: flex;
					justify-content: start;
					flex-direction: row;
					align-items: center;
					margin-left: 1rem;
					margin-right: 1rem;

					input {
						margin-left: 0.7rem;
						margin-right: 0rem;
						width: 100%;
					}
				}
			}
		}
	}

</style>
