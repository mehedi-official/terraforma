<script>
	import { arrow_up_right } from '@components/icons/Icons.svelte';
</script>

<nav class="text-primary-100 flex items-start justify-between">
	<ul
		class="hidden items-center gap-6 *:text-base/normal *:hover:underline-offset-2 *:not-even:hover:underline sm:flex"
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

	<button>{@render arrow_up_right()}</button>
</nav>
