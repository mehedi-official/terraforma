<script lang="ts">
	import { arrow_left, arrow_right } from '@components/icons/Icons.svelte';
	import Card from './Card.svelte';
	import service_banner from '$lib/assets/service-banner.jpg';
</script>

<section class="text-primary-200 bg-[#DFD5CD] p-4">
	<section class="flex flex-col gap-16">
		<div class="grid grid-cols-[7fr_9.5fr]">
			<h1>Services</h1>
			<div class="mt-11 flex items-end justify-between gap-4">
				<h2 class="max-w-128 text-5xl tracking-tight">
					Crafting Sustainable Solutions for Every Space
				</h2>
				<a href="/" class="uppercase underline underline-offset-4">View All</a>
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

	<section class="mt-4 grid grid-cols-3 gap-4">
		<Card />
		<Card />
		<Card />
	</section>

	<section class="banner mt-4 flex min-h-176 flex-col gap-4 pt-40 text-center text-white">
		<p>Insight</p>
		<h2 class="text-7xl">Build Your <br /> Sustainable Space</h2>
	</section>
</section>

<style>
	.banner {
		background: url('$lib/assets/service-banner.jpg');
	}
</style>
