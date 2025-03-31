<script lang="ts">
	import about_us from '$lib/assets/about-us-image.jpg';
	import { arrow_right } from '@components/icons/Icons.svelte';
</script>

<section class="text-primary-200 grid gap-6 bg-[#E4DCD5] p-4 sm:gap-0">
	<div class="flex flex-col gap-12">
		<div class="flex flex-col-reverse justify-between gap-4 sm:flex-row sm:items-end">
			<h2 class="max-w-240 font-serif text-4xl sm:text-6xl">
				At TerraForma, we are dedicated to designing sustainable living spaces that harmonize with
				nature and inspire eco-conscious lifestyles
			</h2>
			<h1 class="text-lg/normal">About us</h1>
		</div>
		<button
			class="flex aspect-square w-10 items-center justify-center bg-[#3C240D] text-white sm:self-end"
			>{@render arrow_right()}</button
		>
	</div>

	<section class="flex flex-col justify-between gap-12 sm:flex-row">
		<div class="flex max-w-104 flex-col justify-between gap-3">
			<p class="text-justify font-sans text-base">
				We believe in shaping a greener future by blending cutting-edge design with sustainable
				practices. From energy-efficient structures to the thoughtful use of natural materials,
				every project we undertake is a step toward preserving the environment for generations to
				come.
			</p>
			<a href="/" class="text-lg/normal font-normal uppercase underline underline-offset-4"
				>Learn More</a
			>
		</div>
		<div class="flex flex-col items-end">
			<img
				src={about_us}
				alt="About us banner"
				class="aspect-9/4 object-cover sm:max-w-135 2xl:aspect-9/6"
			/>
		</div>
	</section>
</section>
