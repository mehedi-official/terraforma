<script lang="ts">
	import { arrow_left, arrow_right } from '@components/icons/Icons.svelte';
	import Card from './Card.svelte';
	import service_banner from '$lib/assets/service-banner.jpg';
</script>

<section class="text-primary-200 bg-[#DFD5CD] p-4">
	<section class="flex flex-col gap-16">
		<div class="grid sm:grid-cols-[7fr_9.5fr]">
			<h1 class="text-lg/normal">Services</h1>
			<div class="mt-11 flex flex-col justify-between gap-4 sm:flex-row sm:items-end">
				<h2 class="max-w-132 font-serif text-5xl sm:text-6xl">
					Crafting Sustainable Solutions for Every Space
				</h2>
				<a href="/" class="text-lg/normal uppercase underline underline-offset-4">View All</a>
			</div>
		</div>
		<div class="flex gap-3 self-end">
			<button class="flex aspect-square w-10 items-center justify-center bg-[#3C240D]"
				>{@render arrow_left()}</button
			>
			<button class="flex aspect-square w-10 items-center justify-center bg-[#3C240D]"
				>{@render arrow_right()}</button
			>
		</div>
	</section>

	<section class="mt-4 grid gap-4 sm:grid-cols-3">
		<Card />
		<Card />
		<Card />
	</section>

	<section
		class="banner mt-4 flex min-h-146 flex-col gap-4 pt-40 text-center text-white sm:min-h-176"
	>
		<p class="text-lg/normal">Insight</p>
		<h2 class="font-serif text-5xl sm:text-8xl">Build Your <br /> Sustainable Space</h2>
	</section>
</section>

<style>
	.banner {
		background: url('$lib/assets/service-banner.jpg');
	}
</style>
