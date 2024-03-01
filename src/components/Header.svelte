<script>
	export let y;

	let tabs = [
		{name: "Home", link: "#home"},
		{name: "About", link: "#about"},
		{name: "Skills", link: "#skills"},
		{name: "Projects", link: "#projects"},
	];

	let prevY;
	let clientHeight;

	const deriveDirection = (pY) => {
		const direction = !prevY || prevY < pY ? 'down' : 'up';
		prevY = pY;

		return direction;
	}


	$: scrollDirection = deriveDirection(y);
	$: offscreen = scrollDirection === 'down' && y > clientHeight * 3;

</script>


<header 
	bind:clientHeight
	class={"sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between " + (
		y > 0 ? " py-4  backdrop-blur" : " py-6 bg-transparent border-transparent"
	)}
	class:-translate-y-full={offscreen} 
	>
	<div class={"absolute top-0 left-0 z-[-10] w-full h-full " + (
		y > 0 ? "bg-[#16161a] opacity-90" : " "
	)}>
	</div>
	<h1 class="font-medium">
		<b class="font-bold poppins">Fadi</b> Ayad
	</h1>
	<div class="sm:flex items-center gap-12 hidden ml-10">
		{#each tabs as tab, index}
			<a href={tab.link} class="duration-200 text-[#fffffe] hover:text-[#7f5af0] hover:font-semibold">
				<p class={"poppins " + (
					tab.name == "Home" ? "text-[#2cb67d] font-semibold" : " "
				)}>{tab.name}</p>
			</a>
		{/each}
	</div>

	<a 
		href="#"
		target="_blank" 
		class="hidden sm:flex relative px-4 py-2 group text-[#fffffe] bg-[#7f5af0] hover:bg-[#2cb67d] duration-200 shadow"
	>
		<div class="absolute top-[5px] w-full h-full bg-[#2cb67d] z-[-1] left-[4px] group-hover:translate-y-[-10px] group-hover:bg-[#7f5af0] duration-200" />

		<h4 class="relative z-9 poppins font-semibold text-[#fffffe] ">
			Get in touch
			<i class="fa-solid fa-envelope ml-2" />
		</h4>
	</a>


</header>