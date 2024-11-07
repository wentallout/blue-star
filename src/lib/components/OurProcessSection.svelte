<section class="operate g-pad">
	<div class="operate__content">
		<h2 id="our-process" class="operate__title">this is how we operate</h2>
		<button class="operate__button">Free AI Consultation</button>
	</div>

	<div class="operate__steps">
		<article class="step">
			<div class="step__number">01</div>
			<h3 class="step__title">Discover & Analyze</h3>
			<p class="step__description">
				We start by diving deep into your business to identify processes and tasks that could be
				replaced by or enhanced with AI.
			</p>
			<div class="step__illustration"></div>
		</article>

		<article class="step">
			<div class="step__number">02</div>
			<h3 class="step__title">Build & Implement</h3>
			<p class="step__description">
				Then, we develop AI-driven solutions and automations tailored to your processes and
				seamlessly integrate them into your workflow.
			</p>
			<div class="step__illustration"></div>
		</article>

		<article class="step">
			<div class="step__number">03</div>
			<h3 class="step__title">Manage & Improve</h3>
			<p class="step__description">
				We start by diving deep into your business to identify processes and tasks that could be
				replaced by- or enhanced with AI.
			</p>
			<div class="step__illustration"></div>
		</article>
	</div>
</section>

<style>
	.operate__steps {
		display: grid;
		grid-template-columns: 1fr;
		gap: var(--space-m);

		.step {
			padding: 50px;
			border: 1px solid grey;
		}
	}

	@media (min-width: 768px) {
		.operate__steps {
			grid-template-columns: 1fr 1fr 1fr;
		}
	}

	.operate__content {
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		align-items: center;
	}

	.step__number {
		color: blue;
		font-size: 64px;
		margin-bottom: var(--space-s);
		font-weight: 600;
	}

	.step__title {
		font-size: var(--step-2);
		font-weight: 500;
		margin-bottom: 18px;
	}
</style>
