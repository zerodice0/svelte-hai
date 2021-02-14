<script>
	import {Router, Link, Route} from 'svelte-routing'
	import Login from './routes/Login.svelte'
	import About from './routes/About.svelte'
	export let url = "";
</script>

<Router url={url}>
	<nav class="navigation">
		<Link class="link" to="/">Home</Link>
		<Link class="link" to="/about">About</Link>
	</nav>
	<div class="router-content">
		<Route path="/" component="{Login}"/>
		<Route path="/about" component="{About}"/>
	</div>
</Router>

<style lang="scss">
	.navigation {
		display: flex;
		flex-direction: row;
		justify-content: start;
		align-items: center;
		height: 3rem;
		border-radius: 7px;
		padding: 5px;
		background: #ededed;
		box-shadow: inset 14px 14px 28px #afafaf,
					inset -14px -14px 28px #ffffff;
	

	}


	.router-content {
		width: 100%;
		height: 100%;
	}
</style>