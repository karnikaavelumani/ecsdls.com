<script lang="ts">
	interface Partnership {
		name: string;
		image: string;
		darkImage?: string;
		link: string;
	}

	const partnerships: Partnership[] = [
		{
			name: 'Raytheon Technologies',
			image: '/assets/raytheon.svg',
			link: 'https://www.rtx.com/'
		},
		{
			name: 'CSUF Engineering and Computer Science',
			image: '/assets/csufecs.png',
			link: 'http://www.fullerton.edu/ecs/'
		},
		{
			name: 'Southern California Edison International',
			image: '/assets/edison.svg',
			link: 'https://www.sce.com/'
		},
		{
			name: 'Hyundai',
			image: '/assets/hyundai.svg',
			link: 'https://www.hyundaiusa.com/us/en'
		},
		{
			name: 'Chevron',
			image: '/assets/chevron.svg',
			link: 'https://www.chevron.com/'
		},
		{
			name: 'Blizzard Entertainment',
			image: '/assets/blizzard-light.svg',
			darkImage: '/assets/blizzard-dark.svg',
			link: 'https://www.blizzard.com/en-us/'
		}
	];
</script>

<section class="partnerships-section">
	<h2 id="partnerships-title">Our partnerships</h2>
	<div class="partnerships-container">
		{#each partnerships as partnership}
			<div class="partnerships-logo">
				<a href={partnership.link}>
					<!-- <img
						src={isDarkMode && partnership.darkImage ? partnership.darkImage : partnership.image}
						alt={partnership.name + ' Logo'}
					/> -->
					<picture>
						{#if partnership.darkImage}
							<!-- Image for light mode -->
							<source srcset={partnership.image} media="(prefers-color-scheme: light)" />
							<!-- Image for dark mode -->
							<source srcset={partnership.darkImage} media="(prefers-color-scheme: dark)" />
						{/if}
						<!-- Fallback image for browsers that don't support the picture element -->
						<img src={partnership.image} alt={partnership.name + ' Logo'} />
					</picture>
				</a>
			</div>
		{/each}
	</div>
</section>

<style>
	.partnerships-section {
		display: grid;
		justify-content: center;
		align-items: center;
	}

	.partnerships-section h2 {
		text-align: center;
	}

	.partnerships-container {
		display: grid;
		grid-template-columns: 1fr 1fr;
		grid-gap: 50px;
		margin: 0 2em 5em;
		align-items: center;
	}

	h2 {
		font-size: var(--size-lg);
		font-weight: 600;
	}

	img {
		width: 100%;
		max-height: 100px;
	}

	@media screen and (min-width: 768px) {
		.partnerships-container {
			display: grid;
			grid-template-columns: 1fr 1fr 1fr;
			grid-gap: 80px;
			margin: 2em;
		}

		img {
			width: 275px;
		}
	}
</style>
