<header class="navbar g-pad">
	<nav class="navbar__nav">
		<div class="navbar__logo">
			<img src="/images/blue-star-logo.avif" alt="" />
			<div class="navbar__title">BlueStar</div>
		</div>

		<ul class="navbar__links">
			<li class="navbar__link"><a href="#services">Services</a></li>
			<li class="navbar__link"><a href="#our-process">Our Process</a></li>
			<li class="navbar__link"><a href="#benefits">Benefits</a></li>
			<li class="navbar__link"><a href="#industries">Industries</a></li>
			<li class="navbar__link"><a href="#faq">FAQ</a></li>
		</ul>

		<button class="btn navbar__button">Contact us</button>
	</nav>
</header>

<style>
	.navbar {
		width: 100%;
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
		padding-block: var(--space-s);
	}

	.navbar__links {
		display: none;
	}

	@media (min-width: 768px) {
		.navbar__links {
			display: flex;
			flex-direction: row;

			outline: 1px solid var(--border-dark);
			border-radius: var(--border-radius);
			overflow: hidden;

			.navbar__link {
				display: flex;

				flex-grow: 1;
				transition: all 0.3s ease-in-out;
				border: 1px solid transparent;

				a {
					display: flex;
					width: 100%;
					height: 100%;
					padding: var(--space-xs) var(--space-m);
				}

				&:hover {
					border: 1px solid var(--border-light);
					background-color: var(--background-200);
				}
			}
		}
	}

	.navbar__nav {
		display: flex;
		flex-direction: row;
		width: 100%;
		justify-content: space-between;
		align-items: center;
		gap: 24px;
	}

	.navbar__logo {
		display: flex;
		flex-direction: row;
		justify-items: center;
		align-items: center;
		gap: 16px;

		.navbar__title {
			font-size: 24px;
		}

		img {
			aspect-ratio: 1;
			width: 24px;
			height: 24px;
		}
	}
</style>
