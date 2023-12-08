<script>
	import Header from './Nav.svelte';
	import './styles.css';
	import 'bulma/css/bulma.css';
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<footer class="footer">
		<div class="content has-text-centered">
			<p>footer</p>
		</div>
	</footer>
</div>
