<script>
	import Project from "./Project.svelte";
	import ReverseProject from "./ReverseProject.svelte";


	let steps = [
		{name: 'Ecommerce Management website', icon: 'fa-solid fa-cart-shopping'},
		{name: 'Ultimate Todos', icon: 'fa-solid fa-list-check'},
		{name: 'Pokedex', icon: 'fa-solid fa-diagram-project'},
	]
</script>

<main class="flex flex-col flex-1 p-4">
	<section id="home" class="grid grid-cols-1 lg:grid-cols-2 gap-16 py-12 sm:py-14 md:pl-5">
		<div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
			<h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
				<h2 class="poppins bg-gradient-to-r from-[#2cb67d] to-green-400 inline-block text-transparent bg-clip-text">Fadi </h2>
				Ayad<br/>
				Full-stack <h2 class="poppins bg-gradient-to-r from-[#7f5af0] to-purple-400 inline-block text-transparent bg-clip-text">Developer</h2>
			</h2>

			<p class="w-5/6 md:w-auto mx-auto break-words text-base sm:text-lg md:text-xl mt-2 lg:mt-0 ">
				I develop compelling
				<span class="underline decoration-[#7f5af0]">
					web	
				</span>
				and
				<span class="underline decoration-[#7f5af0]">
					mobile	
				</span>
				experiences, 
				<span class="underline decoration-[#2cb67d] ">
					custom-built	
				</span>
				 apps tailored for your unique needs.
			</p>
			
			<div class="flex flex-col lg:flex-row lg:items-center gap-4 lg:gap-16 mt-4 lg:mt-0 ">
				<a 
					href="#"
					target="_blank" 
					class="mx-auto lg:mx-0 poppins lg:ml-0 text-base sm:text-lg md:text-xl relative px-4 py-2 group text-[#fffffe] bg-[#7f5af0] hover:bg-[#2cb67d] duration-200 shadow  mb-3 lg:mt-0"
				>
					<div class="absolute top-[4px] w-[96%] h-full bg-[#2cb67d] z-[-1] left-[2%] group-hover:translate-y-[-9px] group-hover:bg-[#7f5af0] duration-200" />

					<h4 class="relative z-9 poppins  font-semibold text-[#fffffe] ">
						Get in touch
						<i class="fa-solid fa-envelope ml-2" />
					</h4>
				</a>

				<div class="flex justify-center gap-4 lg:gap-8 ">
					<i class="text-xl lg:text-2xl fa-brands fa-github"></i>
					<i class="text-xl lg:text-2xl fa-brands fa-linkedin"></i>
					<i class="text-xl lg:text-2xl fa-brands fa-upwork"></i>
					<i class="text-xl lg:text-2xl fa-brands fa-whatsapp"></i>
				</div>
			</div>
		</div>

		<div class="relative grid place-items-center mt-6">
			<img src={"images/avatar.webp"} alt="avatar image" class="object-cover z-{2} max-h-[70vh]" />
		</div>

	</section>

	<section id="projects" class="py-8 lg:py-32 flex flex-col gap-24">
		<div class="flex flex-col text-center">
			<h6 class="text-md sm:text-xl md:text-2xl">
				some things i've built
			</h6>
			<h3 class="font-semibold text-2xl sm:text-4xl md:text-5xl">
				Curious to <h2 class="poppins bg-gradient-to-r from-[#2cb67d] to-green-400 inline-block text-transparent bg-clip-text">see</h2> my work?
			</h3>

		</div>

		
		
		
	</section>
</main>