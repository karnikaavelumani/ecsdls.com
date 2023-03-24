<section class="core-activities-section">
	<h2 id="core-activities">Our core activities</h2>
	<div class="core-activities-container">
		<div class="core-activity-content">
			<h3 id="keynote-speakers">Keynote speakers</h3>
			<p>
				Our keynote speakers offer unique insights and perspectives focused on the event's theme,
				leaving a lasting impact on attendees and empowering them to lead and effect change in their
				communities.
			</p>
		</div>

		<div class="core-activity-content photo">
			<img src="/assets/speaker.svg" alt="Frog speaker" />
		</div>

		<div class="core-activity-content">
			<h3 id="panelists">Panelists</h3>
			<p>
				Our industry experts will answer your questions, draw on their experience to guide you, and
				provide valuable advice to help you succeed. Join us to learn, engage, and network with
				peers and professionals!
			</p>
		</div>

		<div class="core-activity-content photo">
			<img src="/assets/panelist.svg" alt="Animal panelists" />
		</div>
	</div>
</section>

<!-- TODO:
  - [ ] Swap content with illustration for odd rows.
  - [ ] Center all the text!
  
  Reference:
  - https://www.figma.com/file/XThxubY4v3KuDMrU6QOuwO/ecsdls.com?node-id=14-114&t=ABDxmZ8B6AdW2SFY-0 -->
<style>
	.core-activities-section {
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	.core-activities-section h2 {
		text-align: center;
	}

	.core-activities-container {
		display: grid;
		grid-template-columns: 1fr 1fr;
		grid-template-rows: repeat(n, auto);
		grid-gap: 20px;
		width: min(80vw, 70ch);
	}

	.core-activity-content {
		display: flex;
		flex-direction: column;
		text-align: center;
	}

	.photo {
		width: max-content;
		height: max-content;
	}

	/* .core-activity-illustration {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
	} */

	.core-activity-content img {
		align-self: center;
		justify-self: center;
		width: 200px;
	}

	h2 {
		font-size: var(--size-xl);
	}

	h3 {
		font-size: var(--size-lg);
		margin: 0;
	}

	p {
		font-size: large;
	}

	@media screen and (min-width: 768px) {
	}
</style>
