<script lang="ts">
  import { onMount } from 'svelte';

  let isScrolled = false;

  onMount(() => {
    const handleScroll = () => {
      isScrolled = window.scrollY > 10;
    };
    window.addEventListener('scroll', handleScroll);
    return () => window.removeEventListener('scroll', handleScroll);
  });
</script>

<header class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 {isScrolled ? 'bg-white/80 backdrop-blur-md border-b border-gray-100 py-3' : 'bg-transparent py-5'}">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex items-center justify-between">
    <div class="flex items-center gap-8">
      <a href="/" class="flex items-center gap-2 text-2xl font-bold text-gray-900 tracking-tight">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-gray-900">
          <path d="M12 2L2 7L12 12L22 7L12 2Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M2 17L12 22L22 17" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M2 12L12 17L22 12" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
        Lindy
      </a>
      
      <nav class="hidden md:flex items-center gap-6">
        <button class="text-sm font-medium text-gray-600 hover:text-gray-900 flex items-center gap-1">
          Product
          <svg width="10" height="6" viewBox="0 0 10 6" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M1 1L5 5L9 1" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </button>
        <button class="text-sm font-medium text-gray-600 hover:text-gray-900 flex items-center gap-1">
          Solutions
          <svg width="10" height="6" viewBox="0 0 10 6" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M1 1L5 5L9 1" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </button>
        <a href="#" class="text-sm font-medium text-gray-600 hover:text-gray-900">Enterprise</a>
        <a href="#" class="text-sm font-medium text-gray-600 hover:text-gray-900">Pricing</a>
        <button class="text-sm font-medium text-gray-600 hover:text-gray-900 flex items-center gap-1">
          Resources
          <svg width="10" height="6" viewBox="0 0 10 6" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M1 1L5 5L9 1" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </button>
      </nav>
    </div>

    <div class="flex items-center gap-4">
      <a href="#" class="text-sm font-medium text-gray-600 hover:text-gray-900">Log in</a>
      <a href="#" class="text-sm font-medium text-gray-900 bg-white border border-gray-200 hover:bg-gray-50 px-4 py-2 rounded-full transition-colors">Talk to sales</a>
      <a href="#" class="text-sm font-medium text-white bg-blue-600 hover:bg-blue-700 px-4 py-2 rounded-full transition-colors">Try for free</a>
    </div>
  </div>
</header>
