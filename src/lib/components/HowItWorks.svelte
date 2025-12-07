<script>
  // No script needed for static layout
</script>

<section class="py-24 bg-white">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    
    <!-- Header -->
    <div class="flex flex-col md:flex-row md:items-end justify-between mb-12 gap-6">
      <div>
        <div class="flex items-center gap-2 text-gray-500 font-medium mb-4">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect x="3" y="3" width="18" height="18" rx="2" stroke="currentColor" stroke-width="2"/>
            <path d="M8 12h8" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
            <path d="M12 8v8" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
          </svg>
          <span>Easy as one, two, three.</span>
        </div>
        <h2 class="text-3xl md:text-4xl font-bold text-gray-900">How it works.</h2>
      </div>
      <button class="bg-blue-600 text-white px-5 py-2.5 rounded-full font-medium hover:bg-blue-700 transition-colors flex items-center gap-2">
        Try for free
        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
      </button>
    </div>

    <!-- Cards Grid -->
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
      
      <!-- Card 1: Describe your agent -->
      <div class="bg-white rounded-2xl border border-gray-200 overflow-hidden flex flex-col h-full">
        <div class="bg-[#FDF4FF] h-48 relative flex items-center justify-center p-6 overflow-hidden">
          <!-- Background Grid Pattern -->
          <div class="absolute inset-0 opacity-10" style="background-image: radial-gradient(#A855F7 1px, transparent 1px); background-size: 20px 20px;"></div>
          
          <!-- Chat UI -->
          <div class="relative w-full max-w-[240px]">
            <div class="bg-white rounded-2xl rounded-tr-none p-3 shadow-sm border border-purple-100 mb-4 ml-auto w-fit">
              <div class="flex items-center gap-2 text-purple-600 font-medium text-sm">
                <span>Automate everything</span>
                <div class="w-5 h-5 bg-purple-100 rounded-full flex items-center justify-center">
                  <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 19V5"/><path d="m5 12 7-7 7 7"/></svg>
                </div>
              </div>
            </div>
            <div class="bg-purple-100 rounded-2xl rounded-tl-none p-2 w-fit shadow-sm">
              <span class="text-xs font-bold text-purple-800 px-2">Lindy</span>
            </div>
          </div>
        </div>
        <div class="p-6 flex-1">
          <div class="flex items-baseline gap-2 mb-2">
            <span class="text-4xl font-bold text-gray-200">1</span>
            <h3 class="text-xl font-bold text-gray-900">Describe your agent</h3>
          </div>
          <p class="text-gray-600 text-sm leading-relaxed">
            Ask Lindy what to do and watch it build your Agent in minutes.
          </p>
        </div>
      </div>

      <!-- Card 2: Connect your apps -->
      <div class="bg-white rounded-2xl border border-gray-200 overflow-hidden flex flex-col h-full">
        <div class="bg-[#F0FDF4] h-48 relative flex items-center justify-center p-6 overflow-hidden">
          <!-- App Grid -->
          <div class="grid grid-cols-3 gap-3 transform rotate-[-5deg] scale-110">
             <!-- Zoom -->
             <div class="w-10 h-10 bg-white rounded-xl shadow-sm flex items-center justify-center text-blue-500">
               <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M14 10.174V5.5a1.5 1.5 0 0 0-1.5-1.5h-9A1.5 1.5 0 0 0 2 5.5v13A1.5 1.5 0 0 0 3.5 20h9a1.5 1.5 0 0 0 1.5-1.5v-4.674l5 3.889a1 1 0 0 0 1.611-.79V7.075a1 1 0 0 0-1.611-.79l-5 3.889Z"/></svg>
             </div>
             <!-- Slack -->
             <div class="w-10 h-10 bg-white rounded-xl shadow-sm flex items-center justify-center">
               <svg width="20" height="20" viewBox="0 0 24 24" fill="none"><rect x="4" y="4" width="16" height="16" rx="3" fill="#4A154B"/><path d="M9.5 9.5h5v5h-5v-5z" fill="white"/></svg>
             </div>
             <!-- OpenAI -->
             <div class="w-10 h-10 bg-white rounded-xl shadow-sm flex items-center justify-center text-gray-800">
                <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M22.2819 9.8211a5.9847 5.9847 0 0 0-.5157-4.9108 6.0462 6.0462 0 0 0-6.5098-2.9A6.0651 6.0651 0 0 0 4.9807 4.1818a5.9847 5.9847 0 0 0-3.9977 2.9 6.0462 6.0462 0 0 0 .7427 7.0966 5.98 5.98 0 0 0 .511 4.9107 6.051 6.051 0 0 0 6.5146 2.9001A5.9847 5.9847 0 0 0 13.2599 24a6.0557 6.0557 0 0 0 5.7718-4.2058 5.9894 5.9894 0 0 0 3.9977-2.9001 6.0557 6.0557 0 0 0-.7475-7.0729zm-9.022 12.6081a4.4755 4.4755 0 0 1-2.8764-1.0408l.1419-.0804 4.7783-2.7582a.7948.7948 0 0 0 .3927-.6813v-6.7369l2.02 1.1686a.071.071 0 0 1 .038.052v5.5826a4.504 4.504 0 0 1-4.4945 4.4944zm-9.6607-4.1254a4.4708 4.4708 0 0 1-.5346-3.0137l.142.0852 4.783 2.7582a.7712.7712 0 0 0 .7806 0l5.8428-3.3685v2.3324a.0804.0804 0 0 1-.0332.0615L9.74 19.9502a4.4992 4.4992 0 0 1-6.1408-1.6464zM2.3408 7.8956a4.485 4.485 0 0 1 2.3655-1.9723V11.6a.7664.7664 0 0 0 .3879.6765l5.8144 3.3543-2.0201 1.1685a.0757.0757 0 0 1-.071 0l-4.8303-2.7865A4.504 4.504 0 0 1 2.3408 7.872zm16.5963 3.8558L13.1038 8.364 15.1192 7.2a.0757.0757 0 0 1 .071 0l4.8303 2.7913a4.4944 4.4944 0 0 1-.6765 8.1042v-5.6772a.79.79 0 0 0-.407-.667zm2.0107-3.0231l-.142-.0852-4.7735-2.7818a.7759.7759 0 0 0-.7854 0L9.409 9.2298V6.8974a.0662.0662 0 0 1 .0284-.0615l4.8303-2.7866a4.4992 4.4992 0 0 1 6.6802 4.66zM8.3065 12.863l-2.02-1.1638a.0804.0804 0 0 1-.038-.0567V6.0742a4.4992 4.4992 0 0 1 7.3757-3.4533l-.142.0805L8.704 5.4596a.7948.7948 0 0 0-.3927.6813zm1.09-1.107l4.5742-2.6444 4.5742 2.6444-4.5742 2.6444z"/></svg>
             </div>
             <!-- Notion -->
             <div class="w-10 h-10 bg-white rounded-xl shadow-sm flex items-center justify-center text-black">
               <span class="font-serif font-bold text-xl">N</span>
             </div>
             <!-- Google Drive -->
             <div class="w-10 h-10 bg-white rounded-xl shadow-sm flex items-center justify-center">
               <svg width="20" height="20" viewBox="0 0 24 24" fill="none"><path d="M8.5 17H15.5L22 5.5H15L8.5 17Z" fill="#FFC107"/><path d="M2 5.5L5.5 11.5L8.5 17L15 5.5H8L2 5.5Z" fill="#4CAF50"/><path d="M8 5.5H15L18.5 11.5L22 5.5H8Z" fill="#1976D2"/></svg>
             </div>
             <!-- More placeholders -->
             <div class="w-10 h-10 bg-white rounded-xl shadow-sm flex items-center justify-center text-gray-400">
               <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/></svg>
             </div>
          </div>
        </div>
        <div class="p-6 flex-1">
          <div class="flex items-baseline gap-2 mb-2">
            <span class="text-4xl font-bold text-gray-200">2</span>
            <h3 class="text-xl font-bold text-gray-900">Connect your apps</h3>
          </div>
          <p class="text-gray-600 text-sm leading-relaxed">
            Thousands of integrations available.
          </p>
        </div>
      </div>

      <!-- Card 3: Let AI do the work -->
      <div class="bg-white rounded-2xl border border-gray-200 overflow-hidden flex flex-col h-full">
        <div class="bg-gradient-to-br from-pink-50 to-purple-50 h-48 relative flex items-center justify-center p-6 overflow-hidden">
          <div class="bg-white rounded-xl shadow-sm p-4 w-full max-w-[220px] transform rotate-2">
            <div class="text-xs text-gray-400 mb-2">Email body</div>
            <div class="space-y-2">
              <div class="flex gap-2">
                <div class="w-3 h-3 rounded-full bg-purple-200 mt-1"></div>
                <div class="flex-1 space-y-1">
                  <div class="h-2 bg-gray-100 rounded w-full"></div>
                  <div class="h-2 bg-gray-100 rounded w-5/6"></div>
                  <div class="h-2 bg-purple-100 rounded w-full"></div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="p-6 flex-1">
          <div class="flex items-baseline gap-2 mb-2">
            <span class="text-4xl font-bold text-gray-200">3</span>
            <h3 class="text-xl font-bold text-gray-900">Let AI do the work</h3>
          </div>
          <p class="text-gray-600 text-sm leading-relaxed">
            Give custom instructions to your agent, all in natural language.
          </p>
        </div>
      </div>

    </div>
  </div>
</section>
