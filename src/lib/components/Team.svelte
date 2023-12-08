<script>
	import monke from '$lib/assets/monke.svg';

	let people = [
		{ name: 'Bob', year: '4', bio: 'hi', image: monke },
		{ name: 'Bob', year: '4', bio: 'hi', image: monke },
		{ name: 'Bob', year: '4', bio: 'hi', image: monke },
		{ name: 'Bob', year: '4', bio: 'hi', image: monke }
	];

</script>

<div>
		<div class="columns is-multiline">
			{#each people as person}
				<div class="column is-one-quarter">
					<div class="card">
						<div class="card-image">
							<figure class="image is-4by3">
								<img src={person.image} alt={`Picture of ${person.name}`} />
							</figure>
						</div>
						<div class="card-content">
							<div class="media">
								<div class="media-content">
									<p class="title is-4">{person.name}</p>
									<p class="subtitle is-6">{person.year}</p>
								</div>
							</div>
							<div class="content">
								{person.bio}
							</div>
						</div>
					</div>
				</div>
			{/each}
		</div>
	</div>