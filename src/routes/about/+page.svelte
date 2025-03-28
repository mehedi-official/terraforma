<script lang="ts">
	const themes = ['default', 'dark', 'blue'];

	let selectedTheme = $state(themes[0]);

	function changeTheme(theme: string) {
		selectedTheme = theme;
	}
</script>

<main class="theme-{selectedTheme}">
	<section class="mx-16 grid gap-6">
		<h1 class=" text-primary text-5xl">
			Creating timeless spaces with minimal environmental impact, transforming the way we live, the
			one green space at a time.
		</h1>

		<div>
			<p class=" text-primary">
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Quos similique esse labore
				voluptates porro maiores magnam ipsa laudantium natus, ipsum voluptatem, aut asperiores
				soluta, veniam accusamus et quibusdam enim. Asperiores.
			</p>
		</div>

		<button class=" bg-primary px-5 py-3 text-white">Sign up</button>
	</section>

	<div class="mt-24 flex gap-8">
		{#each themes as theme}
			<button
				onclick={() => changeTheme(theme)}
				class="bg-primary cursor-pointer px-4 py-2 text-white">{theme}</button
			>
		{/each}
	</div>
</main>
