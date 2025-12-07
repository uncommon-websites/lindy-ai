<script>
  // Static
</script>

<section class="py-24 bg-white overflow-hidden">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 mb-16">
    <div class="flex items-center justify-between">
      <div>
        <div class="flex items-center gap-2 text-gray-500 font-medium mb-4">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect x="3" y="3" width="18" height="18" rx="2" stroke="currentColor" stroke-width="2"/>
            <path d="M8 12h8" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
            <path d="M12 8v8" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
          </svg>
          <span>Integrations</span>
        </div>
        <h2 class="text-3xl md:text-4xl font-bold text-gray-900">
          Integrates with all your apps.
        </h2>
      </div>
      <a href="#" class="text-gray-600 hover:text-gray-900 font-medium hidden md:block">Browse all integrations</a>
    </div>
  </div>

  <!-- Isometric Grid -->
  <div class="relative h-[400px] w-full flex justify-center items-center perspective-[1000px]">
    <div class="grid grid-cols-8 gap-6 transform rotate-x-[30deg] rotate-y-[-10deg] rotate-z-[10deg] scale-110 origin-center">
      {#each Array(32) as _, i}
        <div class="w-20 h-20 bg-white rounded-2xl shadow-lg border border-gray-100 flex items-center justify-center hover:-translate-y-2 transition-transform duration-300">
          {#if i === 12}
             <!-- Lindy Logo Center -->
             <div class="w-24 h-24 bg-[#FFF9E5] rounded-2xl flex items-center justify-center border-4 border-white shadow-xl z-10 absolute -top-2 -left-2">
                <svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" class="text-gray-900"><path d="M12 2L2 7L12 12L22 7L12 2Z"/><path d="M2 17L12 22L22 17"/><path d="M2 12L12 17L22 12"/></svg>
             </div>
          {:else}
             <!-- Random Icon Placeholders -->
             <div class="w-10 h-10 rounded-full bg-gray-50 flex items-center justify-center text-gray-400">
               <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5"><circle cx="12" cy="12" r="10"/></svg>
             </div>
          {/if}
        </div>
      {/each}
    </div>
    
    <!-- Fade overlay -->
    <div class="absolute inset-0 bg-gradient-to-t from-white via-transparent to-transparent pointer-events-none"></div>
    <div class="absolute inset-0 bg-gradient-to-b from-white via-transparent to-transparent pointer-events-none"></div>
  </div>
</section>

<style>
  .perspective-\[1000px\] {
    perspective: 1000px;
  }
  .rotate-x-\[30deg\] {
    transform: rotateX(30deg) rotateY(-10deg) rotateZ(10deg) scale(1.1);
  }
</style>
