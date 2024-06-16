<script lang="ts">
	import { TextGenerateEffect } from '$components/TextGenerateEffect';
	import Example from '$components/ThreeDCardEffect/Example.svelte';
</script>

<div class="mt-8 text-center text-neutral-500">
	<TextGenerateEffect
		words="Hi, I'm Ozan, I'm a Full Stack Engineer. I build bespoke web applications and websites. Check some of these out below!"
	/>
</div>
<div class="mt-8 dark:bg-primary sm:hidden md:block lg:block">
	<Example />
</div>

<a href="https://linktr.ee/ozancaglar96" target="_blank">
	<div class="dark:bg-neutral grid place-items-center bg-primary">
		<TextGenerateEffect
			className="mb-4"
			words="Interested in working with me? Click this banner for my linktr.ee"
		/>
	</div>
</a>
