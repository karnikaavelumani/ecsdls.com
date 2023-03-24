<section class="core-activities-section">
	<div class="core-activities-container">
		<h2 id="core-activities">Our core activities</h2>
		<div class="core-activity-container">
			<div class="core-activity-content">
				<h3 id="keynote-speakers">Keynote speakers</h3>
				<p>
					Our keynote speakers offer unique insights and perspectives focused on the event's theme,
					leaving a lasting impact on attendees and empowering them to lead and effect change in
					their communities.
				</p>
			</div>
			<div class="core-activity-illustration">
				<img src="/assets/speaker.svg" alt="Frog speaker" />
			</div>
		</div>

		<div class="core-activity-container">
			<div class="core-activity-content">
				<h3 id="panelists">Panelists</h3>
				<p>
					Our industry experts will answer your questions, draw on their experience to guide you,
					and provide valuable advice to help you succeed. Join us to learn, engage, and network
					with peers and professionals!
				</p>
			</div>
			<div class="core-activity-illustration">
				<img src="/assets/panelist.svg" alt="Animal panelists" />
			</div>
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

	.core-activities-container {
		display: flex;
		flex-direction: column;
		gap: 42px;
		width: min(80vw, 50ch);
	}

	.core-activities-container h2 {
		text-align: center;
	}

	.core-activity-container {
		display: flex;
		flex-direction: column;
		gap: 42px;
	}

	.core-activity-content {
		text-align: center;
	}

	.core-activity-illustration {
		text-align: center;
	}

	.core-activity-illustration img {
		width: 175px;
	}

	h2 {
		font-size: xxx-large;
	}
	h3 {
		font-size: x-large;
	}

	@media screen and (min-width: 768px) {
		.core-activity-container {
			flex-direction: row;
			width: min(80vw, 50ch);
		}

		.core-activity-container:nth-child(odd) {
			flex-direction: row-reverse;
		}
	}
</style>
