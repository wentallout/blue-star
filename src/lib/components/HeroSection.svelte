<section class="hero g-pad">
	<img class="hero__img" src="/images/blue-star-logo.avif" alt="" />

	<h1 class="hero__title">We grow your business using artificial intelligence.</h1>

	<div class="hero__btns">
		<button class="btn hero__btn">Consultation</button>
		<button class="btn hero__btn">Free eBook</button>
	</div>
</section>

<style>
	.hero {
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		min-height: 90dvh;
	}

	.hero__btns {
		display: flex;
		justify-content: center;
		align-items: center;
		width: 100%;
		gap: var(--space-m);
	}

	.hero__title {
		text-wrap: pretty;
		font-size: var(--step-5);
		text-align: center;
		line-height: 120%;
		font-weight: 400;
		margin-bottom: var(--space-m);
	}

	.hero__img {
		width: 30%;
		aspect-ratio: 1/1;
		height: auto;
		margin-bottom: var(--space-m);
	}
</style>
