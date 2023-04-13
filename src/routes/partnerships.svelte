<section class="partnerships-section">
	<h2 id="partnerships">Our partnerships</h2>
	<div class="partnerships-container">
		<div class="partnerships-logo">
			<a href="https://www.rtx.com/">
				<img src="/assets/raytheon.svg" alt="Raytheon Technologies Logo" />
			</a>
		</div>

		<div class="partnerships-logo">
			<a href="http://www.fullerton.edu/ecs/">
				<img src="/assets/csufecs.png" alt="CSUF Engineering and Computer Science Logo" />
			</a>
		</div>

		<div class="partnerships-logo">
			<a href="https://www.sce.com/">
				<img src="/assets/edison.svg" alt="Southern California Edison International Logo" />
			</a>
		</div>

		<div class="partnerships-logo">
			<a href="https://www.hyundaiusa.com/us/en">
				<img src="/assets/hyundai.svg" alt="Hyundai Logo" />
			</a>
		</div>

		<div class="partnerships-logo">
			<a href="https://www.chevron.com/">
				<img src="/assets/chevron.svg" alt="Chevron Logo" />
			</a>
		</div>

		<div class="partnerships-logo">
			<a href="https://www.blizzard.com/en-us/">
				<img src="/assets/blizzard.svg" alt="Blizzard Entertainment Logo" />
			</a>
		</div>
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
		grid-gap: 30px;
		margin: 0 2em 2em;
		/* align-items: center;
		justify-items: center;
		text-align: center;
		grid-gap: 60px;
		width: 80%;
		margin: 2em; */
	}

	h2 {
		font-size: var(--size-lg);
		font-weight: 600;
	}

	img {
		width: 100%;
	}

	@media screen and (min-width: 768px) {
		.partnerships-container {
			display: grid;
			grid-template-columns: 1fr 1fr 1fr;
			grid-gap: 60px;
			margin: 2em;
		}

		img {
			width: 275px;
			max-height: fit-content;
		}
	}
</style>
