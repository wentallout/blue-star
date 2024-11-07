<script lang="ts">
	let clients = [
		{
			name: 'E-commerce',
			desc: `Customer support systems: we build omnichannel AI-based customer support systems, consisting of chatbots that operate 24/7 and seamlessly handle your customer support tasks such as providing product recommendations, providing tracking details, accepting returns, and answering FAQ's. Reducing your time spent on customer support by 90% while delivering an outstanding level of customer service. All for the cost of a single customer service employee.`
		},
		{
			name: 'Agencies',
			desc: `AI-driven lead generation: we automate key parts of agencies' outreach to generate more qualified leads and secure more clients with less effort.
Automated content creation: using AI, we empower agencies to automate their content creation, resulting in more impactful messaging and increased viewer engagement.
Staff training chatbots: we build AI-driven chatbots that utilize your SOP documents to train new staff, ensuring your onboarding process runs smoother than ever. `
		},
		{
			name: 'Real Estate',
			desc: `AI-driven property matching: we leverage AI to match potential buyers or renters with properties tailored to their preferences, leading to heightened conversion rates and increased customer satisfaction.
AI-driven lead generation: we utilize AI to engage with potential clients, capture their details, and to schedule a first meeting. Ensuring more effective first meetings while spending less time on acquiring leads.
Holiday rental customer support chatbots: we build AI-driven chatbots that operate 24/7 and in multiple languages, providing immediate responses to all customer inquiries such as check-in procedures, property issues, and area recommendations, reducing your time spent on customer support by 90%.`
		},
		{
			name: 'Influencers & Coaches',
			desc: `Persona chatbots: too many  Instagram DMs to handle? Our AI-driven chatbots seamlessly integrate with your social media, providing 24/7 instant responses to your followers in a manner indistinguishable from you. Sit back and watch your following grow.
			AI-driven lead generation: finding qualified leads when selling a product on social media can be though. We build custom chatbots that qualify leads and save their details, ensuring you sell to the right audience. 
			Automated content creation: using AI, we empower influencers to automate their content creation, resulting in more impactful messaging and increased viewer engagement.`
		},
		{
			name: 'Finance',
			desc: `Lead generation chatbots: we build AI-driven chatbots that engage and qualify potential clients by answering questions, performing calculations, making recommendations, capturing lead details, and scheduling a first meeting. Ensuring more effective first meetings while spending less time on acquiring leads.
Staff training chatbots: we build AI-driven chatbots that utilize your SOP documents to train new staff, ensuring your onboarding process runs smoother than ever. `
		}
	];

	let selectedClient = clients[0]; // Default to the first client

	function selectClient(index: number) {
		selectedClient = clients[index];
	}
</script>

<section class="client g-pad">
	<h2 class="client__title">Who we work with</h2>

	<div class="client__count"><span class="dot"></span>Taking on 3 clients/month</div>

	<div class="client__content">
		<div class="client__list">
			{#each clients as client, index}
				<button class="client__item" on:click={() => selectClient(index)}>{client.name}</button>
			{/each}
		</div>
		<div class="client__info">
			<h3 class="client__name">{selectedClient.name}</h3>
			<p class="client__desc">{selectedClient.desc}</p>
		</div>
	</div>
</section>

<style>
	.client__count {
		padding: 4px 8px;
		border: 1px solid grey;
		width: fit-content;
		margin-inline: auto;
	}

	.client__content {
		display: grid;
		grid-template-columns: 1fr 1fr;
		padding: 75px 60px;
		border: 1px solid grey;
	}

	.client__list {
		display: flex;
		flex-direction: column;
	}

	.client__item {
		cursor: pointer;
		display: flex;
		justify-content: left;
		align-items: center;
	}
</style>
