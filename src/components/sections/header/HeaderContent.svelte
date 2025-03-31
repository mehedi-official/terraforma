<script lang="ts">
	import small_banner from '$lib/assets/header_small_banner.jpg';
	import { arrow_right } from '@components/icons/Icons.svelte';
</script>

<section class="mt-32 grid grid-cols-[3fr_1fr]">
	<section class=" text-primary-200">
		<section class="w-fit">
			<div class="flex justify-between">
				<h1 class=" font-serif text-9xl 2xl:text-9xl">Sustainable</h1>
				<a href="/" class="mt-1 text-lg/normal uppercase underline underline-offset-2"
					>Talk your plan</a
				>
			</div>

			<div class="flex items-end gap-6">
				<h1 class="font-serif text-9xl 2xl:text-9xl">Living</h1>
				<span class="bg-primary-200 h-0.5 w-32"></span>
				<h1 class="font-serif text-9xl 2xl:text-9xl">Spaces</h1>
			</div>
		</section>
	</section>

	<section>
		<div class="relative aspect-square w-28.5">
			<img src={small_banner} alt="Small Banner" class="h-full w-full object-cover" />
			<button
				class="absolute bottom-0 left-0 flex aspect-square w-8 items-center justify-center bg-[#3C240D]"
				>{@render arrow_right()}</button
			>
		</div>

		<p class="text-primary-100 mt-6 text-base">
			Creating timeless spaces with minimal environmental impact, transforming the way we live, the
			one green space at a time.
		</p>
	</section>
</section>
