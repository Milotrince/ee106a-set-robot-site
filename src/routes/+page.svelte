<script>
	import demo from '$lib/assets/demo.mp4';
	import setLogo from '$lib/assets/set-logo.svg';
	import Goal from '$lib/components/Goal.svelte';
	import Design from '$lib/components/Design.svelte';
	import Implementation from '$lib/components/Implementation.svelte';
	import Results from '$lib/components/Results.svelte';
	import Conclusions from '$lib/components/Conclusions.svelte';
	import Team from '$lib/components/Team.svelte';
	import Materials from '$lib/components/Materials.svelte';
</script>

<svelte:head>
	<title>Set Robot - EECS106a</title>
	<meta name="description" content="Berkeley EECS106a Final Project" />
</svelte:head>

<section>
	<div class="section">
		<div class="columns">
			<div class="column is-three-fifths" style="max-width: 600px">
				<video controls autoplay loop style="max-height: 100vh">
					<source src={demo} type="video/mp4" />
					Your browser does not support the video tag.
				</video>
			</div>
			<div class="column">
				<div class="is-flex is-flex-direction-column is-justify-content-center" style="height: 70%">
					<h1 class="is-size-1">
						Our robot plays
						<img src={setLogo} width="200" style="vertical-align: middle" alt="Set" />, the card
						game!
					</h1>
				</div>
			</div>
		</div>
	</div>
	<div class="container px-5">
		<div class="section">
			<h1 class="is-size-1">Project Goal</h1>
			<Goal />
		</div>

		<div class="section">
			<h1 class="is-size-1">Design</h1>
			<Design />
		</div>

		<div class="section">
			<h1 class="is-size-1">Implementation</h1>
			<Implementation />
		</div>

		<div class="section">
			<h1 class="is-size-1">Results</h1>
			<Results />
		</div>

		<div class="section">
			<h1 class="is-size-1">Conclusions</h1>
			<Conclusions />
		</div>

		<div class="section">
			<h1 class="is-size-1">Team</h1>
			<Team />
		</div>

		<div class="section">
			<h1 class="is-size-1">Materials</h1>
			<Materials />
		</div>
	</div>
</section>
