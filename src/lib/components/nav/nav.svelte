<script>
	const items = ['About', 'Theme', 'Professionals', 'Register'];
</script>

<header class="header">
	<div class="header__left">
		<a href="/" class="header__brand">
			<img src="/logo.svg" class="header__logo" alt="Logo" />
			<span class="header__brand-text">ECS Summit</span>
		</a>
	</div>

	<nav class="header__right">
		<ol class="header__navbar">
			{#each items as name (name)}
				{@const id = name.toLowerCase()}
				<li class="header__navbar-item"><a href={`#${id}`}>{name}</a></li>
			{/each}
		</ol>
	</nav>
</header>

<style>
	.header {
		display: grid;
		grid-template-columns: auto 1fr;
		grid-gap: 5px;
		align-items: center;
		padding: 20px;
	}

	.header__left {
		display: flex;
		align-items: center;
	}

	.header__brand {
		display: flex;
		align-items: center;
	}

	.header__logo {
		width: 50px;
		height: 50px;
		margin-right: 10px;
	}

	.header__brand-text {
		display: none;
	}

	.header__right {
		display: flex;
		justify-content: end;
	}

	.header__navbar {
		align-items: center;
		list-style: none;
		padding: 0;
		margin: 0;
	}

	.header__navbar-item {
		margin-right: 20px;
	}

	@media (min-width: 768px) {
		.header__brand-text {
			display: block;
		}

		.header__navbar {
			display: flex;
			margin: 0;
			padding: 0;
		}
	}
</style>
