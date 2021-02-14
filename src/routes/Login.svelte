<script>
	const login = () => {
		alert("hello");
	}
</script>

<main>
	<div class="simple-modal">
		<div class="mock-bar">
	    
		</div>

		<div class="header">
			<span class="title">HAT</span>
			<span class='subtitle'>How about this?</span>
		</div>
		<div class="body">
			<input type="text"
				placeholder="login id"/>
			<input type="text"
				placeholder="password"/>
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
			/* border: 3px solid black; */
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

				input, button {
					margin-left: 1rem;
					margin-right: 1rem;
				}
			}
		}
	}

</style>
