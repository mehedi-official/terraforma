<script lang="ts">
	import project_banner from '$lib/assets/project-banner.jpg';
	import { arrow_left, arrow_right } from '@components/icons/Icons.svelte';

	let services = [
		{ name: 'Year Completed', detail: `${new Date().getFullYear()}` },
		{ name: 'Number of Units', detail: '150 eco-friendly residential units' },
		{ name: 'Eco-Friendly Materials', detail: '25% recycled materials' },
		{ name: 'Biophilic Features', detail: '70% green space coverage' },
		{ name: 'Community Facilities', detail: '5 EV charging stations' },
		{ name: 'Waste Management', detail: '100% waste segregation' },
		{ name: 'Carbon Footprint Reduction', detail: '200 ton of CO2 saved annually' },
		{ name: 'Cost Saving for Residents', detail: 'Up to 25% reduction in utility bills' }
	];
</script>

<section class="text-primary-200 grid grid-cols-[2fr_3fr] gap-6 bg-[#DFD5CD] p-4">
	<section class="flex flex-col justify-between gap-6">
		<p class="max-w-110 text-lg">
			Every project reflects our commitment to creating environmentally conscious designs that
			inspire and serve future generations
		</p>
		<div class=" min-h-85 bg-black">
			<img src={project_banner} alt="Project Banner" class="h-full w-full object-cover" />
		</div>
	</section>
	<section>
		<div class="flex justify-between gap-6">
			<h2 class="mt-6 max-w-118 font-serif text-6xl">Innovative Spaces, Designed Sustainably</h2>
			<h1 class="text-lg/normal">Projects</h1>
		</div>
		<section class="border-primary-200 mt-12 border-t">
			{#each services as { name, detail }}
				<div
					class="border-primary-200 flex items-center justify-between gap-4 border-b py-5 text-lg/normal"
				>
					<p>{name}</p>
					<p>{detail}</p>
				</div>
			{/each}
			<!-- <div>
                <p>Year Completed</p>
                <p>{new Date().getFullYear()}</p>
            </div>
            <div>
                <p>Number of Units</p>
                <p>150 eco-friendly residential units</p>
            </div>
            <div>
                <p>Eco-Friendly Materials</p>
                <p>25% recycled materials</p>
            </div>
            <div>
                <p>Biophilic Features</p>
                <p>70% green space coverage</p>
            </div>
            <div>
                <p>Community Facilities</p>
                <p>5 EV charging stations</p>
            </div>
            <div>
                <p>Waste Management</p>
                <p>100% waste segregation</p>
            </div>
            <div>
                <p>Carbon Footprint Reduction</p>
                <p>200 ton of CO2 saved annually</p>
            </div>
            <div>
                <p>Cost Saving for Residents</p>
                <p>Up to 25% reduction in utility bills</p>
            </div> -->
		</section>
	</section>
</section>

<div class="text-primary-200 flex items-end justify-between gap-6 bg-[#DFD5CD] px-4 pt-6 pb-4">
	<div class="flex gap-3">
		<button class="flex aspect-square w-10 items-center justify-center bg-[#3C240D]"
			>{@render arrow_left()}</button
		>
		<button class="flex aspect-square w-10 items-center justify-center bg-[#3C240D]"
			>{@render arrow_right()}</button
		>
	</div>
	<a href="/" class="uppercase underline underline-offset-4">View All</a>
</div>
