<script lang="ts">
	import imgWelcome from '$lib/assets/img/IMG_0997.png';
	import IconDownFill from '$lib/components/icons/down-fill.svelte';
</script>

<div
	id="ctn.inicio"
	class="m-0 px-2 pb-12 flex relative left-0 right-0 w-full min-h-[95vh] h-screen items-center justify-center align-middle"
>
	<div class="flex flex-col w-full h-full md:w-[95%] lg:w-[90%] xl:w-[85%] m-auto p-0 justify-center align-middle items-center gap-12">
		<!-- Imagen -->
		<div class="relative w-full h-auto flex justify-center items-center overflow-hidden m-0 mt-12 lg:mt-0 p-0 pt-8 md:pt-10">
			<div class="absolute inset-0 z-0 flex w-full justify-center items-center select-none pointer-events-none px-0 lg:px-12 pb-12 lg:pb-0">
				<h1 
                    style="font-size: clamp(80px, 15vw, 200px);"
                class="w-full lg:w-auto relative left-0 font-bold italic uppercase text-slate-400 opacity-30 backdrop-opacity-40 backdrop-blur-sm text-start leading-[0.85]">
					Full <br />
					<span class="font-black not-italic">Stack</span>
				</h1>
			</div>
			<img
				id=""
				class="relative z-10 max-w-150 w-full h-auto object-contain saturate-100 contrast-120 hover:scale-105 transform-gpu transition-all duration-300 ease-in-out"
				alt="Retrato"
				src={imgWelcome}
			/>
		</div>
		<p
			class="w-full h-auto text-md md:text-lg lg:text-xl font-regular text-justify uppercase text-white font-[Nunito_Code] opacity-80 backdrop-opacity-0 leading-relaxed"
		>
			Transformo ideas en experiencias digitales robustas. Especialista en desarrollo con
			<span class="underline text-orange-400 opacity-100">Svelte</span>
			y 
            <span class="underline text-indigo-400 opacity-100">JSP</span>, integrando
			<span class="underline">Inteligencia Artificial</span>
			para optimizar procesos y crear soluciones innovadoras.
		</p>
		<div class="w-full h-auto flex flex-col lg:flex-row lg:gap-auto justify-center lg:justify-between items-center align-middle">
			<button
				id="show.cv"
				class="p-3 px-5 m-0 bg-slate-800 rounded-full hover:-translate-y-2 hover:translate-x-2 ocus:outline-2 focus:outline-offset-2 focus:outline-[#49824B] active:bg-[#49824B] transition-all transform-content duration-150 ease-in-out"
				on:click={() => console.log('click')}
			>
				<span class="text-white opacity-80">Echa un vistazo a mi CV</span>
			</button>
			<IconDownFill class="flex relative justify-center items-center w-8 h-8 text-white opacity-80 top-16 lg:top-0 bottom-0" />
			<ul class="hidden lg:flex flex-row gap-x-8">
				<li>Github</li>
				<li>LinkedIn</li>
				<li>Behance</li>
			</ul>
		</div>
	</div>
</div>
