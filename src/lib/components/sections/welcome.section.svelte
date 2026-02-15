<script lang="ts">
	import imgWelcome from '$lib/assets/img/IMG_0997.png';
</script>

<div
	id="ctn.inicio"
	class="m-0 px-2 flex flex-col w-full min-h-[98vh] h-screen items-center justify-between align-middle"
>
	<div
		class="flex flex-col w-full h-full max-h-[90%] md:w-[95%] lg:w-[90%] xl:w-[85%] justify-center align-middle items-center text-center gap-12"
	>
        <!-- Imagen -->
		<div class="relative w-full h-auto flex justify-center items-center overflow-hidden m-0 pt-8 md:pt-10">
			<div class="absolute inset-0 z-0 flex justify-center items-center select-none pointer-events-none px-12">
				<h1 class="text-[15vw] md:text-[9vw] font-extrabold uppercase text-white opacity-50 text-start md:text-center leading-[0.85]">
					Full Stack<br />Developer
				</h1>
			</div>
			<img
				id=""
				class="relative z-10 w-auto max-h-100 object-contain saturate-70 contrast-150 hover:scale-105 transform-gpu transition-all duration-300 ease-in-out"
				alt="Retrato"
				src="/src/lib/assets/img/IMG_0997.png?t=1771167054421"
			/>
		</div>
		<p class="w-full h-auto text-2xl font-regular uppercase text-slate-400 font-[Nunito_Code] opacity-50 backdrop-opacity-0">
			Apasionado de la programación y el diseño web. Especializado en el desarrollo web con JSP y Svelte
		</p>
		<div class="w-full h-auto flex flex-row gap-auto justify-between items-center align-middle">
			<a
				id="show.cv"
				class=""
				target="_blank"
				rel="noopener noreferrer"
				href=""
			>
				Echa un vistazo a mi CV
			</a>
			<p>Enlaces a redes corporativas: Github, Linkedin, Behance</p>
		</div>
	</div>
</div>
