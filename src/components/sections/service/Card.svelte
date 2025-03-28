<script lang="ts">
	import { arrow_right } from '@components/icons/Icons.svelte';
</script>

<section class="flex min-h-132 flex-col justify-between bg-[#E4DCD5] p-4">
	<h3 class="text-5xl">Sustainable Architecture Design</h3>

	<div class="flex flex-col gap-3">
		<p class=" text-justify">
			Our experts guide you through the process of creating environmentally structures that align
			with your goals.
		</p>
		<button
			class="flex aspect-square w-10 cursor-pointer items-center justify-center self-end bg-[#FE784C] hover:bg-[#3C240D]"
			>{@render arrow_right()}</button
		>
	</div>
</section>
