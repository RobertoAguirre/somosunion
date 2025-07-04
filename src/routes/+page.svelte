<script lang="ts">
	const imagenes = [
		"/logo.png",
		"https://placehold.co/900x400/8A3677/fff?text=Impacto",
		"https://placehold.co/900x400/00ACA6/fff?text=Comunidad",
		"https://placehold.co/900x400/B28A39/fff?text=Oportunidad"
	];
	let actual = 0;
	function siguiente() { actual = (actual + 1) % imagenes.length; }
	function anterior() { actual = (actual - 1 + imagenes.length) % imagenes.length; }
</script>

<!-- CARRUSEL GRANDE -->
<section class="relative min-h-[50vh] flex items-center justify-center bg-gris">
	<img src={imagenes[actual]} alt="Hero Somos" class="absolute inset-0 w-full h-full object-cover opacity-60" />
	<div class="relative z-10 w-full max-w-4xl mx-auto flex flex-col items-center justify-center py-12">
		<div class="flex justify-center gap-2 mb-6">
			<button on:click={anterior} class="bg-morado text-blanco rounded-full p-2 shadow hover:bg-dorado border-2 border-blanco">&#8592;</button>
			<button on:click={siguiente} class="bg-morado text-blanco rounded-full p-2 shadow hover:bg-dorado border-2 border-blanco">&#8594;</button>
		</div>
	</div>
</section>

<!-- SECCIÓN QUIÉNES SOMOS (MORADO) -->
<section class="py-12 border-t-4 text-blanco" style="background-color: #8A3677; border-color: #B28A39;">
	<div class="max-w-5xl mx-auto px-4 grid md:grid-cols-2 gap-10 items-center">
		<div>
			<h2 class="text-2xl md:text-3xl font-bold mb-3" style="color: #B28A39;">¿Quiénes somos?</h2>
			<p class="mb-4 text-justify" style="color: #fff;">
				La creación de esta organización se dio por la existencia de personas expuestas a factores de riesgo asociados a la violencia y la desigualdad social. Promovemos oportunidades dignas y justas.
			</p>
			<ul class="list-disc pl-5 font-medium space-y-1">
				<li style="color: #B28A39;">Desarrollo humano</li>
				<li style="color: #B28A39;">Economía solidaria</li>
				<li style="color: #B28A39;">Reconciliación y perdón</li>
				<li style="color: #B28A39;">Oportunidades justas</li>
			</ul>
		</div>
		<div class="flex justify-center">
			<img src="/logo.png" alt="Logo Somos" class="rounded-full shadow-lg border-4" style="border-color: #00ACA6; background: #fff;" />
		</div>
	</div>
</section>

<!-- SECCIÓN DE CONTACTO (MORADO) -->
<section id="contacto" class="py-12 border-t-4" style="background-color: #f8f5ed; border-color: #B28A39;">
	<div class="max-w-lg mx-auto px-4 rounded-2xl shadow-2xl border border-white/30" style="box-shadow: 0 8px 40px 0 rgba(80, 40, 80, 0.25), 0 1.5px 8px 0 rgba(80, 40, 80, 0.10);">
		<br>
		<h2 class="text-2xl font-bold mb-6 text-center" style="color: #B28A39;">Contacto</h2>
		<form class="flex flex-col gap-5">
			<input type="text" placeholder="Nombre" class="px-5 py-3 rounded-lg border-none bg-white text-morado placeholder-morado/60 shadow focus:outline-none focus:ring-2 focus:ring-turquesa text-lg" required />
			<input type="email" placeholder="Email" class="px-5 py-3 rounded-lg border-none bg-white text-morado placeholder-morado/60 shadow focus:outline-none focus:ring-2 focus:ring-turquesa text-lg" required />
			<input type="tel" placeholder="Teléfono" class="px-5 py-3 rounded-lg border-none bg-white text-morado placeholder-morado/60 shadow focus:outline-none focus:ring-2 focus:ring-turquesa text-lg" />
			<textarea placeholder="Escribe tu mensaje aquí..." class="px-5 py-3 rounded-lg border-none bg-white text-morado placeholder-morado/60 shadow focus:outline-none focus:ring-2 focus:ring-turquesa text-lg resize-none" rows="4" required></textarea>
			<button type="submit" class="mt-2 text-white font-bold py-3 rounded-lg shadow-lg text-lg tracking-wide hover:bg-turquesa transition-colors active:scale-95 focus:outline-none focus:ring-2 focus:ring-morado" style="background-color: #8A3677;">Enviar</button>
		</form>
		<div class="text-center mt-8">
			<p class="font-semibold text-blanco">SOMOS UNIÓN</p>
			<a href="mailto:esperechihuahua@gmail.com" class="underline" style="color: #B28A39;">esperechihuahua@gmail.com</a>
			<p></p>
			<br>
		</div>
	</div>
</section>


