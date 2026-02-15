<script lang="ts">
	var arrSkillText = [
		{
			id: 1,
			text: 'Desarrollo',
			description:
				'Me gusta crear experiencias funcionales y diversas. Actualmente estoy trabajando con Java y Spring Boot. La base de mis aplicaciones son en Svelte y Tauri, tecnologias muy utiles para crear aplicaciones eficientes y modernas.',
			icons: 'Java, Svelte, Tauri',
		},
		{
			id: 2,
			text: 'Diseño',
			description:
				'Con un enfoque importante en UI/UX me centro en diseñar interefaces intuitivas y fluidas, que conecten con los usuarios de manera natural.',
			icons: 'Tailwind, SASS',
		},
		{
			id: 3,
			text: 'Diseño Grafico',
			description:
				'Desde siempre he tenido una pasión por el mundo del diseño grafico y he aprendido a diseñar identidades, logotipos, etc... Me encanta convertir ideas en fotografias, imagenes unicas y atractivas.',
			icons: 'Lightroom, Photoshop, Lunacy',
		},
	];
</script>

<div
	id="ctn.skills"
	class="m-0 px-2 mt-42 lg:pt-0 flex relative left-0 right-0 w-full h-full min-h-[98vh] top-0 bottom-0 items-center justify-center align-middle"
>
	<div
		class="flex flex-col w-full h-full md:w-[95%] lg:w-[90%] xl:w-[85%] m-auto p-0 justify-center align-middle items-center gap-12 font-[Nunito_Code]"
	>
		<div class="flex flex-col w-full h-auto m-auto p-0 justify-center item-center gap-8 lg:gap-12">
			<h1
				id=""
				class="flex relative w-full left-0 text-start text-3xl font-extrabold uppercase"
			>
				Puedo ayudarte con
				<span
					class="tracking-wide"
					style=""
				>
					&nbsp;...
				</span>
			</h1>
			<ul
				id=""
				class="flex flex-col lg:flex-row justify-around items-center align-middle gap-6"
			>
				{#each arrSkillText as skill}
					<li
						class="w-full flex relative h-full top-0 flex-col gap-y-2 uppercase justify-start align-middle justify-items-start place-items-start items-start"
					>
						<p class="text-sm text-slate-400 opacity-70 backdrop-opacity-40 backdrop-blur-sm">0{skill.id}</p>
						<h1 class="text-lg font-semibold text-white opacity-80 backdrop-opacity-40 backdrop-blur-sm">{skill.text}</h1>
						<p class="font-normal text-slate-400 opacity-70 backdrop-opacity-40 backdrop-blur-sm">
							{skill.description}
						</p>
						<p class="text-white relative bottom-0 opacity-80 backdrop-opacity-40 backdrop-blur-sm">{skill.icons}</p>
					</li>
				{/each}
			</ul>
		</div>
		<!-- Frase celebre -->
		<div class="flex flex-col w-full justify-center items-center h-auto text lg:px-12 mb-20">
			<h1 class="text-3xl italic text-justify text-slate-400 opacity-70 backdrop-opacity-40 backdrop-blur-sm">"La fuerza del equipo viene de cada miembro. La fuerza de cada miembro es el equipo"</h1>
			<p class="w-full h-auto text-end text-slate-400 opacity-70 backdrop-opacity-40 backdrop-blur-sm">( Phil Jackson )</p>
		</div>
	</div>
</div>
