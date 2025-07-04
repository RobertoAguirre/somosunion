<script lang="ts">
	import '../app.css';
</script>

<header class="bg-white bg-blanco text-morado shadow-md sticky top-0 z-20  border-gris">
	<div class="max-w-6xl mx-auto flex items-center justify-between px-4 py-3">
		<img src="/logo.png" alt="Logo Somos" class="h-12 w-auto" />
		<nav class="flex gap-6 text-base font-medium">
			<a href="/" class="hover:text-dorado transition-colors">Inicio</a>
			<a href="/programas" class="hover:text-dorado transition-colors">Programas</a>
			<a href="/proyectos" class="hover:text-dorado transition-colors">Proyectos</a>
			<a href="/notas" class="hover:text-dorado transition-colors">Notas</a>
			<a href="/galeria" class="hover:text-dorado transition-colors">Galería</a>
		</nav>
	</div>
</header>

<main class="min-h-[70vh] bg-blanco text-negro">
	<slot />
</main>

<footer class="bg-gris text-blanco mt-10">
	<div class="max-w-6xl mx-auto flex flex-col md:flex-row items-center justify-between px-4 py-8 gap-6 border-t border-white/10">
		<div class="text-center md:text-left">
			<span class="font-semibold text-lg tracking-wide">SOMOS UNIÓN</span><br />
			<a href="mailto:esperechihuahua@gmail.com" class="underline hover:text-dorado transition-colors">esperechihuahua@gmail.com</a>
		</div>
		<div class="flex gap-6 mt-4 md:mt-0 justify-center md:justify-end">
			<a href="#" aria-label="Facebook" class="hover:text-dorado transition-colors" title="Facebook">
				<svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24" class="w-7 h-7">
					<path d="M22.675 0h-21.35C.595 0 0 .592 0 1.326v21.348C0 23.406.595 24 1.325 24h11.495v-9.294H9.692v-3.622h3.128V8.413c0-3.1 1.893-4.788 4.659-4.788 1.325 0 2.463.099 2.797.143v3.24l-1.918.001c-1.504 0-1.797.715-1.797 1.763v2.313h3.587l-.467 3.622h-3.12V24h6.116C23.406 24 24 23.406 24 22.674V1.326C24 .592 23.406 0 22.675 0"/>
				</svg>
			</a>
			<a href="#" aria-label="YouTube" class="hover:text-dorado transition-colors" title="YouTube">
				<svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 24 24" class="w-7 h-7">
					<path d="M23.498 6.186a2.994 2.994 0 0 0-2.112-2.112C19.458 3.5 12 3.5 12 3.5s-7.458 0-9.386.574A2.994 2.994 0 0 0 .502 6.186C0 8.114 0 12 0 12s0 3.886.502 5.814a2.994 2.994 0 0 0 2.112 2.112C4.542 20.5 12 20.5 12 20.5s7.458 0 9.386-.574a2.994 2.994 0 0 0 2.112-2.112C24 15.886 24 12 24 12s0-3.886-.502-5.814zM9.545 15.568V8.432L15.818 12l-6.273 3.568z"/>
				</svg>
			</a>
		</div>
		
	</div>
	<br>
</footer>
