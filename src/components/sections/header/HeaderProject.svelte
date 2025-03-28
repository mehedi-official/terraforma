<script lang="ts">
	import banner from '$lib/assets/hero_banner.png?enhanced';
</script>

<section class="text-primary-200 grid gap-4 py-6">
	<div class="grid grid-cols-[6fr_4fr]">
		<p>Eco retreat villas</p>
		<div class="flex justify-between">
			<p>2023</p>
			<p>Luxury Living</p>
		</div>
	</div>

	<div>
		<enhanced:img src={banner} alt="Banner" class="w-full object-cover" />
	</div>

	<div class="flex items-center justify-between">
		<a href="/">Next Project</a>
		<a href="/">View Project</a>
	</div>
</section>
