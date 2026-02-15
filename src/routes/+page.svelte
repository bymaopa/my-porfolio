<!-- /+page.svelte -->
<script lang="ts">
	import { onMount } from 'svelte';
	import { fade } from 'svelte/transition';

	// Secciones
	import SectionWelcome from '$lib/components/sections/welcome.section.svelte';
	import SectionSkill from '$lib/components/sections/skill.section.svelte';
	import SectionProject from '$lib/components/sections/project.section.svelte';

  // Componentes
  import Background from '$lib/components/background/shape.animated.svelte';
  import Footer from '$lib/components/footer.svelte';

	var ready = $state(false);

	onMount(() => {
		ready = true;
	});
</script>

<div
	id="iframe"
	class="relative z-0 h-full max-h-svh w-full overflow-hidden
    rounded-b-[48px] transform-gpu transition-all bg-transparent
    m-0 p-0 text-slate-100 drop-shadow-2xl shadow-2xl"
	style="-webkit-border-top-left-radius: 24px !important;
    -webkit-border-top-right-radius: 24px !important;
    border-top-left-radius: 24px !important;
    border-top-right-radius: 24px !important;
    /* Fuerza a WebKit a recortar el contenido a la forma del borde */
    -webkit-mask-image: -webkit-radial-gradient(white, black);
    /* ...tus bordes... */
    transform: translateZ(0);"
>
	<!-- 
        Fondo de Pantalla 
        Usamos -z-10 para asegurar que esté detras del contenido
    -->
	<Background />

	<!-- Contenedor Principal -->
	{#if ready}
		<div
			id="if.content"
			class="relative m-0 p-0 flex h-full w-full flex-col items-start justify-start overflow-x-hidden align-baseline z-20"
			in:fade={{ duration: 800, delay: 150 }}
		>
      <!-- Aqui deberia de ir un for que recorra esto cuando se inicialice -->
			<SectionWelcome />
			<SectionSkill />
			<SectionProject />
			<Footer />
		</div>
	{/if}
</div>
