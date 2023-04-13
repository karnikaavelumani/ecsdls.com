<script>
	const items = ['Activities', 'Partnership', 'Speakers', 'Council', 'FAQ'];
</script>

<header class="header">
	<div class="header__left">
		<a href="/" class="header__brand">
			<img src="/assets/logo.svg" class="header__logo" alt="Logo" />
		</a>
	</div>

	<nav class="header__middle">
		<ol class="header__navbar">
			{#each items as name (name)}
				{@const id = name.toLowerCase()}
				<li class="header__navbar-item"><a href={`#${id}`}>{name}</a></li>
			{/each}
		</ol>
	</nav>

	<div class="header__right">
		<button class="header__button"><a href="/">RSVP</a></button>
	</div>

	<div class="menu__icon">
		<button class="menu__item">
			<div class="menu__line1" />
			<div class="menu__line2" />
			<div class="menu__line3" />
		</button>
	</div>
</header>

<style>
	.header {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 10px 0;
		background-color: var(--csuf-blue);
		font-weight: 500;
	}

	a {
		color: var(--perma-white);
		text-decoration: none;
		font-size: var(--size-sm);
	}

	.header__middle {
		display: flex;
		justify-content: center;
	}

	.header__navbar {
		display: flex;
		align-items: center;
		list-style: none;
		padding: 0;
		margin: 0;
		gap: 50px;
	}

	.header__left {
		display: flex;
		align-items: center;
		margin-left: 3vw;
		margin-right: 3vw;
	}

	.header__brand {
		display: flex;
		align-items: center;
	}

	.header__logo {
		width: 50px;
		height: 50px;
	}

	.header__right {
		display: flex;
		justify-content: end;
		margin-left: 3vw;
		margin-right: 3vw;
	}

	.header__button {
		background-color: var(--ecs-bluer);
		color: var(--perma-white);
		padding: 0.4rem 1rem;
		border-radius: 10px;
		font-weight: 700;
		border: none;
	}

	.header__navbar-item {
		margin-right: 20px;
	}

	.menu__icon {
		display: none;
	}

	@media (min-width: 900px) {
		.header__navbar {
			display: flex;
			margin: 0;
			padding: 0;
		}
	}
</style>
