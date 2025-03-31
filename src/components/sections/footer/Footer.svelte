<script lang="ts">
	import { arrow_up_right } from '@components/icons/Icons.svelte';
</script>

<section class="text-primary-200 flex justify-between bg-[#E4DCD5] p-4 pb-36">
	<h1 class="max-w-200 font-serif text-9xl">Create Your Sustainable Space</h1>
	<div>{@render arrow_up_right()}</div>
</section>

<footer class="relative overflow-hidden bg-[#3C240F] p-4 text-white/90">
	<section class="flex flex-col justify-between gap-80">
		<section class="flex flex-col gap-6">
			<div class="font-serif text-5xl">Terraforma</div>
			<p class="max-w-110 text-base">
				We believe in shaping a greener future by blending cutting-edge design with sustainable
				practices.
			</p>
		</section>

		<section>
			<ul
				class="flex items-center gap-6 text-base/normal *:hover:underline-offset-2 *:not-even:hover:underline"
			>
				<li><a href="/">About us</a></li>
				<span>/</span>
				<li><a href="/">Services</a></li>
				<span>/</span>
				<li><a href="/">Insights</a></li>
				<span>/</span>
				<li><a href="/">Projects</a></li>
				<span>/</span>
				<li><a href="/">Blog</a></li>
			</ul>
		</section>
	</section>

	<span class="absolute right-6 bottom-0 translate-y-8 font-serif text-9xl text-[#4E3624]"
		>Terraforma</span
	>
</footer>
