<script>

	import {Link, Router, Route } from 'svelte-routing';


	import Index from './Index.svelte';

	import Page1 from './Page1.svelte';
	import Page2 from './Page2.svelte';
	export let url = "";

</script>

<main>

<Router url="{url}">
	<Link to="/">index</Link>
	<Link to="/page1">page1</Link>
	<Link to="/page2">page2</Link>

	<Route path="/page1" component={Page1} />
	<Route path="/page2" component={Page2} />
	<Route path="/" component={Index} />

</Router>

</main>

<style>
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
</style>