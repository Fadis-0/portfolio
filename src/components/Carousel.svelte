<script>
	import emblaCarouselSvelte from 'embla-carousel-svelte';
</script>

<style>
	.embla__slide {
		flex: 0 0 100%;
	}

</style>

<div class="w-2/3 mx-auto embla overflow-hidden rounded" use:emblaCarouselSvelte>
	<div class="embla__container flex">
		<div class="embla__slide min-w-0 shadow-xl bg-white opacity-10 rounded mr-10 h-96 flex items-center justify-center text-black"></div>
		<div class="embla__slide min-w-0 shadow-xl bg-white opacity-10 rounded mr-10 h-96 flex items-center justify-center text-black"></div>
		<div class="embla__slide min-w-0 shadow-xl bg-white opacity-10 rounded h-96 flex items-center justify-center text-black"></div>
	</div>
	<div class="embla__dots"></div>
</div>