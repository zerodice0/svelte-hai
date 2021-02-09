<script>
	
</script>

<main>
	<div class="simple-modal">
		<div class="header">
			<span class="title">HAI</span>
			<span class='subtitle'>How about it?</span>
		</div>
		<div class="body">
			<input type="text"/>
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
			border: 3px solid black;
			border-radius: 4px;
			box-shadow: 3px 5px rgba($color: #000000, $alpha: 0.3);
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

				.title {
					font-size: 1.5rem;
				}
			}

			.body {
				display: flex;
				justify-content: center;
			}
		}
	}

</style>