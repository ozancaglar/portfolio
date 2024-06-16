<script lang="ts">
	import CardBody from './CardBody.svelte';
	import CardContainer from './CardContainer.svelte';
	import CardItem from './CardItem.svelte';

	let isMouseEntered = false;
</script>

<CardContainer bind:isMouseEntered className="inter-var w-4/6 h-svh -mt-8">
	<CardBody
		className="bg-primary-content relative group/card !w-full h-1/2 dark:hover:shadow-2xl dark:hover:shadow-emerald-500/[0.1] dark:bg-neutral dark:border-white/[0.2] border-black/[0.1] w-auto sm:w-[30rem] h-auto rounded-xl p-6 border"
	>
		<CardItem
			{isMouseEntered}
			translateZ="50"
			className="text-xl font-bold text-neutral-600 dark:text-neutral-300"
		>
			<p>NailsByZee</p>
		</CardItem>
		<CardItem
			{isMouseEntered}
			translateZ="60"
			className="text-neutral-500 text-md max-w-sm mt-2 dark:text-neutral-200"
		>
			<p class="text-left">
				Svelte Frontend + Go Backend. Webapp which stores data via either user input or admin manual
				inputs with GDPR compliance functionality.
			</p>
		</CardItem>
		<CardItem {isMouseEntered} translateZ="100" className="w-full mt-4">
			<img
				src="nailsbyzee.webp"
				class="w-full rounded-xl object-cover group-hover/card:shadow-xl"
				alt="thumbnail"
			/>
		</CardItem>
		<div class="flex items-center justify-between">
			<CardItem
				{isMouseEntered}
				translateZ={20}
				className="px-4 py-2 rounded-xl text-xs font-normal dark:text-white"
			>
				<!-- Try now → -->
			</CardItem>
			<CardItem class="mt-4" {isMouseEntered} translateZ={20}>
				<a href="https://nailsbyzee.co.uk/" target="_blank"
					><button class="btn btn-primary">Check it out</button></a
				>
			</CardItem>
		</div>
	</CardBody>
</CardContainer>
