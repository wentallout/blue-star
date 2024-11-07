<script>
	import { TablerBrandLinkedin, TablerBrandInstagram, TablerBrandYoutube } from '$lib/icons';
</script>

<footer class="footer g-pad">
	<div class="footer__logo">
		<img width="24" height="24" src="/images/blue-star-logo.avif" alt="" />
		<div class="">BlueStar</div>
	</div>

	<div class="footer__link">
		<a href="">Terms & conditions</a>
		<a href="">Privacy Policy</a>
		<div class="social">
			<a class="social__icon" href="#">
				<TablerBrandLinkedin width="20" height="20" />
			</a>
			<a class="social__icon" href="#">
				<TablerBrandInstagram width="20" height="20" />
			</a>
			<a class="social__icon" href="#">
				<TablerBrandYoutube width="20" height="20" />
			</a>
		</div>
	</div>
</footer>

<style>
	.footer {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		padding-block: 24px;
	}

	.footer__logo {
		display: flex;
		flex-direction: row;
		align-items: center;
		gap: 12px;
	}

	.footer__link {
		display: flex;
		flex-direction: row;
		align-items: center;
		gap: 24px;
	}

	.social {
		display: flex;
		flex-direction: row;
		gap: 1rem;
	}

	.social__icon {
		background-color: purple;
		border: 1px solid grey;
		aspect-ratio: 1;
		width: 40px;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>
