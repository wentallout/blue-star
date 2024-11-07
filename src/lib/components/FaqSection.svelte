<script>
	// Define the FAQ object containing questions and answers
	let faqs = [
		{
			question: 'Is my company a good fit for BlueStar Automations?',
			answer:
				'We work with businesses of all sizes, and our solutions are tailored to meet your specific needs. Contact us for a consultation to see if we’re a good fit.',
			isOpen: false // Track the open/closed state of each FAQ item
		},
		{
			question: "I don't know what automations I need?",
			answer:
				'Our team will work with you to analyze your processes and identify areas where automation can be beneficial.',
			isOpen: false
		},
		{
			question: 'Is it costly to incorporate automations into my business?',
			answer:
				'The cost varies depending on the complexity of the solutions. We offer scalable options to fit different budgets.',
			isOpen: false
		},
		{
			question: 'How long does it take to implement automations into my business?',
			answer:
				'Implementation time can vary based on the solution. We provide a timeline during the consultation process.',
			isOpen: false
		},
		{
			question: 'How will you assist my team in understanding the implemented technologies?',
			answer:
				'We offer training sessions and ongoing support to ensure your team is comfortable with the new technologies.',
			isOpen: false
		},
		{
			question: 'What support do you offer after deployment?',
			answer: 'We provide continuous support and maintenance to ensure your systems run smoothly.',
			isOpen: false
		}
	];

	// Function to toggle the open/closed state of a FAQ item
	function toggleAnswer(index) {
		faqs[index].isOpen = !faqs[index].isOpen;
	}
</script>

<section class="faq g-pad">
	<h2 id="faq" class="faq__title">Frequently Asked Questions</h2>
	{#each faqs as { question, answer, isOpen }, index}
		<div class="faq__item">
			<button class="faq__question" on:click={() => toggleAnswer(index)}>
				{question}
			</button>
			{#if isOpen}
				<div class="faq__answer">
					<p>{answer}</p>
				</div>
			{/if}
		</div>
	{/each}
</section>

<style>
	.faq {
		margin: auto;

		border-radius: 8px;
		box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
		padding: 20px;
	}

	.faq__title {
		font-size: 2rem;
		margin-bottom: 20px;
		text-align: center;
	}

	.faq__item {
		margin-bottom: 10px;
	}

	.faq__question {
		width: 100%;
		padding: 15px;
		background: #007bff;
		color: white;
		border: none;
		border-radius: 5px;
		text-align: left;
		cursor: pointer;
		font-size: 1.1rem;
	}

	.faq__question:hover {
		background: #0056b3;
	}

	.faq__answer {
		padding: 10px;
		border: 1px solid #e0e0e0;
		border-radius: 5px;
		margin-top: 5px;
	}
</style>
