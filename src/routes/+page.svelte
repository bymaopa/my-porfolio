<!-- /+page.svelte -->
<script lang="ts">
    
    import { onMount } from 'svelte';
	import { fade } from 'svelte/transition';

	var ready = $state(false);

	onMount(() => {
		ready = true;
	});

</script>


<div
	id="iframe"
	class="relative z-0 h-full max-h-svh w-full overflow-y-auto rounded-t-[24px] rounded-b-[48px] border-0 bg-transparent 
    m-0 p-0 text-slate-100 drop-shadow-2xl shadow-2xl"
>
    <!-- 
        Fondo de Pantalla 
        Usamos -z-10 para asegurar que esté detras del contenido
    -->
	<div 
        id="if.background"
        class="absolute inset-0 w-full h-full top-0 right-0 left-0 overflow-hidden"
    >
        <!-- Noise Image -->
        <div class="absolute inset-0 bg-[url(https://grainy-gradients.vercel.app/noise.svg)] mix-blend-overlay opacity-100 z-20 brightness-100 contrast-120"></div>
        <!-- Fondo del iFrame animado -->
        <div id="bg.animated" class="bg-shape-content container-backdrop-blur">
            <div></div>
            <div></div>
            <div></div>
            <div></div>
        </div>
    </div>

    <!-- Contenedor Principal -->
    {#if ready}
	<div
		id="if.content"
		class="relative m-0 p-0 flex h-full w-full flex-col items-start justify-start overflow-auto overflow-x-hidden overflow-y-auto align-baseline z-20"
        in:fade={{ duration: 800, delay: 150 }}
    >   
        <div 
            id="ctn.inicio"
            class="m-0 px-2 w-full min-h-screen h-full items-start justify-start"
        >
            <!-- Imagen mia de Bad Bunny -->
            <p>Mario Ortega</p>
            <h1>Full Stack Developer y Diseño UX</h1>
            <p>Apasionado de la programación y el diseño web. Especializado en el desarrollo web con JSP y Svelte</p>
            <a id="show.cv" href="#">Echa un vistazo a mi CV</a>
			<p>
				Enlaces a redes corporativas: Github, Linkedin, Behance
			</p>
        </div>
        <div 
            id="ctn.skill"
            class="m-0 px-2 w-full min-h-screen h-full items-start justify-start"
        >
            <p>Habilidades</p>
            <h1>Puedo ayudarte con</h1>
            <ul>
                <li>
                    <p>01</p>
                    <h1>Desarrollo</h1>
                    <p>Me gusta crear experiencias funcionales y diversas.</p>
                </li>
                <li>
                    <p>02</p>
                    <h1>Diseño</h1>
                    <p></p>
                </li>
                <li>
                    <p>03</p>
                    <h1>Diseño Grafico</h1>
                    <p></p>
                </li>
            </ul>
            <h1>Una combinacion de creatividad y Habilidades tecnicas es lo necesario para conseguir interfaces unicas</h1>
        </div>
        <div 
            id="ctn.project"
            class="m-0 px-2 w-full min-h-screen h-full items-start justify-start"
        >
            <!-- Listado de proyectos -->
            <h1>Proyectos recientes</h1>
        </div>
        <div 
            id="ctn.contact"
            class="m-0 p-0 w-full max-h-screen h-full inset-0 left-0 right-0 bottom-0 items-start justify-start bg-black"
        >

<footer class="w-full text-white py-16 px-6 md:px-12 lg:px-24 font-sans">
  <div class="max-w-7xl mx-auto flex flex-col md:flex-row justify-between gap-16 md:gap-8">
    
    <div class="flex flex-col justify-end items-start gap-6 order-last md:order-first md:w-1/3">
      
      <div class="w-12 h-12 bg-white rounded-full flex items-center justify-center overflow-hidden mb-2">
        <svg viewBox="0 0 24 24" class="w-8 h-8 text-black fill-current">
          <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 17.93c-3.95-.49-7-3.85-7-7.93 0-.62.08-1.21.21-1.79L9 15v1c0 1.1.9 2 2 2v1.93zm6.9-2.54c-.26-.81-1-1.39-1.9-1.39h-1v-3c0-.55-.45-1-1-1H8v-2h2c.55 0 1-.45 1-1V7h2c1.1 0 2-.9 2-2v-.41c2.93 1.19 5 4.06 5 7.41 0 2.08-.8 3.97-2.1 5.39z"/>
        </svg>
      </div>

      <div class="space-y-1">
        <p class="text-lg font-medium">
          © 2026 
          <span class="bg-linear-to-r from-amber-100 via-yellow-200 to-lime-200 bg-clip-text text-transparent font-bold">
            maopa.
          </span>
        </p>
        <p class="text-gray-500 text-sm">Hecho con pasión y dedicación &lt;3</p>
      </div>
    </div>

    <div class="flex flex-col gap-12 md:w-2/3 lg:pl-32">
      
      <div class="grid grid-cols-1 sm:grid-cols-2 gap-10">
        
        <div class="flex flex-col gap-6">
          <h3 class="text-gray-500 text-xs uppercase tracking-widest font-semibold">Secciones</h3>
          <nav class="flex flex-col gap-3">
            <a href="/" class="text-xl hover:text-gray-300 transition-colors">Inicio</a>
            <a href="/proyectos" class="text-xl hover:text-gray-300 transition-colors">Proyectos</a>
            <a href="/sobre-mi" class="text-xl hover:text-gray-300 transition-colors">Sobre Mí</a>
          </nav>
        </div>

        <div class="flex flex-col gap-6">
          <h3 class="text-gray-500 text-xs uppercase tracking-widest font-semibold">Contacto</h3>
          <div class="flex flex-col gap-3">
            <a href="https://linkedin.com" target="_blank" class="text-xl flex items-center gap-1 hover:text-gray-300 transition-colors">
              Linkedin
            </a>
            <a href="mailto:ydefuente@gmail.com" class="text-xl hover:text-gray-300 transition-colors">mario.ortega.pal@gmail.com</a>
            <a href="tel:+34635372397" class="text-xl hover:text-gray-300 transition-colors">+34 622 539 883</a>
          </div>
        </div>
      </div>

      <div class="flex flex-col gap-6">
        <h3 class="text-gray-500 text-xs uppercase tracking-widest font-semibold">Social</h3>
        <div class="flex flex-wrap gap-6 text-lg font-medium">
          <a href="#" class="text-[#b96ce6] hover:opacity-80 transition-opacity">Github</a>
          <a href="#" class="text-[#3b82f6] hover:opacity-80 transition-opacity">Linkedin</a>
          <a href="#" class="text-[#2563eb] hover:opacity-80 transition-opacity">Behance</a>
        </div>
      </div>

    </div>
  </div>
</footer>
        </div>
	</div>
    {/if}
</div>
