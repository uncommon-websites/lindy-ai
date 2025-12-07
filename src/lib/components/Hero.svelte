<script>
  const chips = [
    { label: 'Personal website', icon: 'M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71' },
    { label: 'Customer Support', icon: 'M21 11.5a8.38 8.38 0 0 1-.9 3.8 8.5 8.5 0 0 1-7.6 4.7 8.38 8.38 0 0 1-3.8-.9L3 21l1.9-5.7a8.38 8.38 0 0 1-.9-3.8 8.5 8.5 0 0 1 4.7-7.6 8.38 8.38 0 0 1 3.8-.9h.5a8.48 8.48 0 0 1 8 8v.5z' },
    { label: 'Outbound Sales Calls', icon: 'M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z' },
    { label: 'Lead gen', icon: 'M16 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2' },
    { label: 'Meeting Recorder', icon: 'M12 1a3 3 0 0 0-3 3v8a3 3 0 0 0 6 0V4a3 3 0 0 0-3-3z' },
    { label: 'LinkedIn outreach', icon: 'M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z' },
    { label: 'Support Chatbot', icon: 'M12 2a2 2 0 0 1 2 2c0 .74-.4 1.39-1 1.73V7h1a7 7 0 0 1 7 7h1a1 1 0 0 1 1 1v3a1 1 0 0 1-1 1h-1v1a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-1H2a1 1 0 0 1-1-1v-3a1 1 0 0 1 1-1h1V7a7 7 0 0 1 7-7z' }
  ];
</script>

<section class="relative pt-32 pb-20 overflow-hidden bg-[#FFFBF0]">
  <!-- Background gradient effects -->
  <div class="absolute top-0 left-1/2 -translate-x-1/2 w-[1000px] h-[600px] bg-[#FFEBB8] opacity-30 blur-[120px] rounded-full pointer-events-none -z-10"></div>

  <div class="max-w-4xl mx-auto px-4 text-center relative z-10">
    
    <!-- Announcement Pill -->
    <div class="inline-flex items-center gap-3 bg-white/60 backdrop-blur-sm border border-gray-200 rounded-full pl-4 pr-1 py-1 mb-8 shadow-sm hover:bg-white/80 transition-colors">
      <span class="text-sm text-gray-700 font-medium">Announcing Lindy Assistant: Put your inbox and meetings on autopilot</span>
      <button class="bg-[#0F172A] text-white text-xs font-semibold px-3 py-1.5 rounded-full hover:bg-gray-800 transition-colors flex items-center gap-1">
        Talk to sales
        <svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M2.5 6H9.5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M6 2.5L9.5 6L6 9.5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
      </button>
    </div>

    <!-- Headline -->
    <h1 class="text-5xl md:text-7xl font-bold text-gray-900 tracking-tight mb-6 leading-[1.1]">
      Meet your first AI employee
    </h1>
    
    <!-- Subheadline -->
    <p class="text-lg text-gray-600 mb-10 max-w-2xl mx-auto">
      Lindy is the simplest way for businesses to create, manage, and share agents. Now with just a prompt.
    </p>

    <!-- Interactive Input -->
    <div class="bg-white rounded-2xl shadow-xl p-2 mb-8 max-w-2xl mx-auto border border-gray-100 relative group">
      <textarea 
        placeholder="How can I help? Describe your agent and I'll build it." 
        class="w-full h-24 p-4 text-lg text-gray-700 placeholder-gray-400 resize-none focus:outline-none rounded-xl"
      ></textarea>
      <div class="absolute bottom-4 right-4">
        <button class="bg-blue-600 hover:bg-blue-700 text-white p-2 rounded-full transition-colors shadow-lg">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M12 19V5" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
            <path d="M5 12L12 5L19 12" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </button>
      </div>
    </div>

    <!-- Quick Action Chips -->
    <div class="flex flex-wrap justify-center gap-3 max-w-3xl mx-auto">
      {#each chips as chip}
        <button class="flex items-center gap-2 bg-white border border-gray-200 px-3 py-1.5 rounded-full text-xs font-medium text-gray-600 hover:border-blue-300 hover:text-blue-600 hover:bg-blue-50 transition-all shadow-sm">
          <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
            <path d={chip.icon} />
          </svg>
          {chip.label}
        </button>
      {/each}
    </div>

  </div>
</section>
