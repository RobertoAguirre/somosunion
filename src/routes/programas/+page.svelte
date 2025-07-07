<script lang="ts">
const programas = [
  {
    titulo: 'Empujoncitos a Negocio',
    imagen: '/img/empujoncitos.jpg',
    descripcion: 'Préstamos ángel para egresados IMESUN que requieren pequeñas inversiones iniciales, con devolución blanda.'
  },
  {
    titulo: 'ESPERES',
    imagen: '/img/espere.jpg',
    descripcion: 'Metodología centrada en el desarrollo humano, sanando heridas y promoviendo una nueva narrativa de vida.'
  },
  {
    titulo: 'Dale Chido',
    imagen: '/img/dalechido.jpg',
    descripcion: 'Actividades terapéuticas, lúdicas y académicas para incrementar habilidades psicosociales y reducir riesgos.'
  },
  {
    titulo: 'Escala',
    imagen: '/img/escala.jpg',
    descripcion: 'Escuela de negocios para emprendedores, formación en gestión empresarial y oportunidades de crecimiento.'
  }
];
</script>

<section class="max-w-6xl mx-auto px-4 py-12">
  <h1 class="text-3xl md:text-4xl font-bold text-morado mb-10 text-center">Programas</h1>
  <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
    {#each programas as p}
      <div class="bg-white rounded-2xl shadow-lg overflow-hidden flex flex-col md:flex-row items-stretch">
        <img src={p.imagen} alt={p.titulo} class="w-full md:w-1/3 h-48 object-cover md:rounded-l-2xl md:rounded-r-none rounded-t-2xl md:rounded-t-none" />
        <div class="flex-1 p-6 flex flex-col justify-between">
          <div>
            <h2 class="text-xl font-bold text-morado mb-2">{p.titulo}</h2>
            <p class="text-gris mb-4">{p.descripcion}</p>
          </div>
        </div>
      </div>
    {/each}
  </div>
</section> 