<script>
  let activeTab = 'Marketing';
  const tabs = [
    { id: 'Support', label: 'Support', desc: 'Handle tickets autonomously.' },
    { id: 'Sales', label: 'Sales', desc: 'Convert more leads' },
    { id: 'Marketing', label: 'Marketing', desc: 'Accelerate campaign execution.' },
    { id: 'Operations', label: 'Operations', desc: 'Turn documents into insights.' }
  ];
</script>

<section class="py-24 bg-white">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    
    <!-- Section Header -->
    <div class="mb-12">
      <div class="flex items-center gap-2 text-gray-500 font-medium mb-4">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
          <rect x="3" y="3" width="18" height="18" rx="2" stroke="currentColor" stroke-width="2"/>
          <path d="M9 9H15" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
          <path d="M9 15H15" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
        </svg>
        <span>Agents</span>
      </div>
      <h2 class="text-3xl md:text-4xl font-bold text-gray-900 max-w-2xl">
        Build, scale, and manage your entire AI workforce with one platform.
      </h2>
    </div>

    <!-- Tabs -->
    <div class="grid grid-cols-1 md:grid-cols-4 gap-4 mb-8">
      {#each tabs as tab}
        <button 
          class="text-left p-4 rounded-xl border transition-all duration-200 {activeTab === tab.id ? 'bg-gray-50 border-gray-200 shadow-sm' : 'bg-white border-transparent hover:bg-gray-50'}"
          on:click={() => activeTab = tab.id}
        >
          <div class="flex items-center justify-between mb-1">
            <span class="font-semibold text-gray-900 flex items-center gap-2">
              {#if tab.id === 'Support'}
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
              {:else if tab.id === 'Sales'}
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2v20M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"/></svg>
              {:else if tab.id === 'Marketing'}
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><circle cx="12" cy="12" r="4"/><line x1="21.17" y1="8" x2="12" y2="8"/><line x1="3.95" y1="6.06" x2="8.54" y2="14"/><line x1="10.88" y1="21.94" x2="15.46" y2="14"/></svg>
              {:else}
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="3"/><path d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1 0 2.83 2 2 0 0 1-2.83 0l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-2 2 2 2 0 0 1-2-2v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83 0 2 2 0 0 1 0-2.83l.06-.06a1.65 1.65 0 0 0 .33-1.82 1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1-2-2 2 2 0 0 1 2-2h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 0-2.83 2 2 0 0 1 2.83 0l.06.06a1.65 1.65 0 0 0 1.82.33H9a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 2-2 2 2 0 0 1 2 2v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 0 2 2 0 0 1 0 2.83l-.06.06a1.65 1.65 0 0 0-.33 1.82V9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 2 2 2 2 0 0 1-2 2h-.09a1.65 1.65 0 0 0-1.51 1z"/></svg>
              {/if}
              {tab.label}
            </span>
            {#if tab.id === 'Marketing'}
              <span class="bg-gray-100 rounded-full p-1">
                <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="6" y="4" width="4" height="16"/><rect x="14" y="4" width="4" height="16"/></svg>
              </span>
            {/if}
          </div>
          <p class="text-sm text-gray-500">{tab.desc}</p>
        </button>
      {/each}
    </div>

    <!-- Main Content Card -->
    <div class="bg-[#F0F6FF] rounded-3xl p-8 md:p-12 border border-blue-50">
      <div class="flex items-center justify-between mb-8">
        <div class="flex items-center gap-3">
          <div class="w-10 h-10 bg-blue-600 rounded-lg flex items-center justify-center text-white">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4.5 16.5c-1.5 1.26-2 5-2 5s3.74-.5 5-2c.71-.84.7-2.13-.09-2.91a2.18 2.18 0 0 0-2.91-.09z"/><path d="m12 15-3-3a22 22 0 0 1 2-3.95A12.88 12.88 0 0 1 22 2c0 2.72-.78 7.5-6 11a22.35 22.35 0 0 1-4 2z"/><path d="M9 12H4s.55-3.03 2-4c1.62-1.08 5 0 5 0"/><path d="M12 15v5s3.03-.55 4-2c1.08-1.62 0-5 0-5"/></svg>
          </div>
          <div>
            <h3 class="text-2xl font-bold text-gray-900">Creative Agent</h3>
            <p class="text-gray-600">Create on brand marketing campaigns with just a prompt.</p>
          </div>
        </div>
        <button class="bg-blue-600 text-white px-5 py-2.5 rounded-full font-medium hover:bg-blue-700 transition-colors flex items-center gap-2">
          Try for free
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
        </button>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
        <!-- Workflow Visualization -->
        <div class="relative pl-8 border-l-2 border-dashed border-blue-200 space-y-8 py-4">
          {#each ['Research competitors', 'Analyze market', 'Generate campaign brief', 'Create ad and video assets'] as step, i}
            <div class="relative">
              <div class="absolute -left-[41px] top-1/2 -translate-y-1/2 w-5 h-5 rounded-full bg-white border-4 border-blue-200"></div>
              <div class="bg-white rounded-lg p-3 shadow-sm border border-gray-100 flex items-center gap-3 w-fit">
                <div class="w-6 h-6 rounded bg-blue-100 flex items-center justify-center text-blue-600">
                  <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/><polyline points="10 9 9 9 8 9"/></svg>
                </div>
                <span class="text-sm font-medium text-gray-700">{step}</span>
              </div>
            </div>
          {/each}
        </div>

        <!-- Placeholder for Result -->
        <div class="bg-white rounded-xl shadow-sm border border-gray-100 p-4 h-full min-h-[300px] flex items-center justify-center relative overflow-hidden">
             <!-- Abstract representation of content -->
             <div class="absolute inset-0 bg-gradient-to-br from-blue-50 to-white opacity-50"></div>
             <div class="w-32 h-40 bg-[#FFEBB8] rounded-lg shadow-sm z-10"></div>
             <div class="absolute right-10 top-10 w-20 h-20 bg-blue-50 rounded-full blur-xl"></div>
        </div>
      </div>
    </div>

  </div>
</section>
