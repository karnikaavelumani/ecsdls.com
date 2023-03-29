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

		<div class="core-activity-content">
			<h3 id="workshops">Workshops</h3>
			<p>
				Collaborate with student leaders in group activities, leverage your skills and experience,
				tackle group tasks, and develop valuable teamwork skills for your future.
			</p>
		</div>
		<div class="core-activity-content photo">
			<img src="/assets/workshops.svg" alt="Paper and tools" />
		</div>

		<div class="core-activity-content">
			<h3 id="mentoring">Speed mentoring</h3>
			<p>
				Engage in 2-on-1 with professionals and peers to ask questions, gain insights, expand
				knowledge, and improve leadership skills. Get a chance to expand your knowledge, build your
				network, and take your leadership skills to the next level.
			</p>
		</div>
		<div class="core-activity-content photo">
			<img src="/assets/mentoring.svg" alt="Animals talking 1 on 1" />
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
		display: grid;
		justify-content: center;
		align-items: center;
	}

	.core-activities-section h2 {
		text-align: center;
	}

	.core-activities-container {
		display: grid;
		/* display: flex;
		flex-direction: column; */
		text-align: center;
		gap: 16px;
		width: 100%;
	}

	.core-activity-content {
		display: grid;
		/* display: flex;
		flex-direction: column; */
		text-align: center;
	}

	.photo img {
		align-self: center;
		justify-self: center;
		width: 200px;
	}

	h2 {
		font-size: var(--size-xl);
		font-weight: 600;
	}

	h3 {
		font-size: var(--size-lg);
		font-weight: 500;
		margin: 0;
	}

	p {
		font-size: var(--size-sm);
	}

	@media screen and (min-width: 768px) {
		.core-activities-container {
			display: grid;
			grid-template-columns: repeat(2, 1fr);
			align-items: center;
			justify-items: center;
			grid-gap: 30px;
			width: min(90vw, 80ch);
			margin-bottom: 2em;
		}

		.core-activity-content:nth-child(1) {
			grid-column: 2;
			grid-row: 1;
		}

		.core-activity-content:nth-child(2) {
			grid-column: 1;
			grid-row: 1;
		}

		.core-activity-content:nth-child(3) {
			grid-column: 2;
			grid-row: 3;
		}

		.core-activity-content:nth-child(4) {
			grid-column: 2;
			grid-row: 2;
		}

		.photo img {
			width: 90%;
		}
	}
</style>
