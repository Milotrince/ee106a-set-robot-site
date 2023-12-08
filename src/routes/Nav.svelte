<script>
	import github from '$lib/assets/github.svg';
	import monke from '$lib/assets/monke.svg';
	let isActive = false;

	function toggleNavbar() {
		isActive = !isActive;
	}
</script>

<header>
	<nav class="navbar is-transparent">
		<div class="navbar-brand">
			<button
				class="navbar-burger"
				data-target="navbarExampleTransparentExample"
				on:click={toggleNavbar}
			>
				<span></span>
				<span></span>
				<span></span>
			</button>
		</div>

		<div class={`navbar-menu ${isActive ? 'is-active' : ''}`}>
			<div class="navbar-start">
				<a class="navbar-item" href="https://ucb-ee106.github.io/eecs106a-fa23site/">
					<img class="navbar-icon" src={monke} alt="EECS C106A Introduction to Robotics" height="28" width="28" />
					EECS C106A
				</a>
				<a class="navbar-item" href="https://github.com/">
					<img class="navbar-icon" src={github} alt="GitHub" height="28" width="28" />
					GitHub
				</a>
			</div>
		</div>
	</nav>
</header>