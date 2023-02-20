<footer class="footer">
	<div class="container">
		<p>Stay connected</p>
	</div>

	<div class="container">
		<p>© 2023 ECS Summit</p>
	</div>

	<div class="container">
		<p>Contact us</p>
	</div>
</footer>

<style>
	.footer {
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		grid-gap: 20px;
		padding: 20px;
		background-color: #333;
		color: #fff;
	}

	.container {
		text-align: center;
	}

	@media (max-width: 600px) {
		.footer {
			grid-template-columns: repeat(1, 1fr);
		}
	}
</style>
