<section class="book g-pad">
	<h2>Free eBook</h2>

	<div class="book__content">
		<img class="book__img" src="/images/ebook.avif" alt="" />

		<div class="book__info">
			<p>
				7 No-code tools used by BlueStar Automations that will instantly streamline your business
				processes and massively cut your time spent on repetitive tasks;
			</p>

			<p>Pro tips and tricks for getting the most out of these tools;</p>

			<p>Examples and instructions on how to seamlessly implement them into your business.</p>

			<p>Get your free copy now to supercharge your operations.</p>

			<input type="text" placeholder="Full name" />
			<input type="text" placeholder="Email" />

			<button>Download eBook</button>
		</div>
	</div>
</section>

<style>
	.book__content {
		display: grid;
		grid-template-columns: 1fr;
	}

	.book__img {
		max-height: 500px;
	}

	.book__info {
		padding: var(--space-xl) var(--space-xl);
		background-color: var(--background-100);
		border-radius: var(--border-radius);
		display: flex;
		flex-direction: column;
		gap: var(--space-m);
		color: var(--text-100);
	}

	@media (min-width: 768px) {
		.book__content {
			grid-template-columns: 1fr 1fr;
		}
	}
</style>
